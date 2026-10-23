# Artifact Signing Client Tools Installer

This MSI package streamlines the installation process for the Artifact Signing client tools for Windows SDK SignTool.exe and all of the dependencies. The installer aims to achieve a one-click installation process on Windows nodes.

Summary of installer actions:
- Bundles the Microsoft Artifact Signing client tools DLLs and all necessary Visual C++ dlib dependencies
- Installs the latest .NET runtime on the client’s machine.
- Incorporates the latest Windows SDK, which houses the essential signtool.exe and its dependencies.

When users decide to uninstall the package the uninstall action removes the Artifact Signing tools, and preserves the .NET runtime and Windows SDK packages.

Please refer MS Learn documentation to [Invoke SignTool to sign a file](https://learn.microsoft.com/en-us/azure/artifact-signing/how-to-signing-integrations#invoke-signtool-to-sign-a-file).

For more information on Artifact Signing refer to [MS Learn Artifact Signing Documentation](https://learn.microsoft.com/en-us/azure/artifact-signing/).

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
trademarks or logos is subject to and must follow 
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.

# Installation Path

If you don't specify an exact path for the artifacts,
they will be installed in the AppData Local directory of your Windows system:

```text
%LOCALAPPDATA%\Microsoft\MicrosoftArtifactSigningClientTools
```

This typically resolves to `C:\Users\<username>\AppData\Local\Microsoft\MicrosoftArtifactSigningClientTools`.
