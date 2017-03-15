# npm using Nexus OPS Toolchain

This echo application uses Node.js and includes a DevOps toolchain that is preconfigured for continuous delivery, source control, and 
integration with a user-provided Nexus server. The OPS toolchain expects to find the modules in the Nexus server, provided by 
the [npm using Nexus Development Toolchain](https://github.com/open-toolchain/dev-npm-toolchain).

To get started, click **Create toolchain**. You will need to fill in five items in the Nexus integration:
- _Integration URL_: The console URL for your Nexus server.
- _User ID_: An appropriate npm email address.
- _Authentication token_: Your npm registry authentication token. For example: `AUTH_TOKEN=$( echo -n nexus_user_id:nexus_password | base64 -w0 - )`
- _Release URL_: Your npm private registry.
- _Mirror or public URL_: Your npm virtual registry that can serve your private registry as well as the Global registry.


[![Deploy To Bluemix](https://console.ng.bluemix.net/devops/graphics/create_toolchain_button.png)](https://console.ng.bluemix.net/devops/setup/deploy/?repository=https%3A//github.com/open-toolchain/ops-npm-toolchain)

For more information about toolchains, see [Custom toolchains in one click with IBM Bluemix DevOps Services](https://developer.ibm.com/devops-services/2016/06/16/open-toolchain-with-ibm-bluemix-devops-services/).

