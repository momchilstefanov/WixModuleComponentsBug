
### Actual Result
Build fails with "ICEM05: The component in the ModuleComponents table does not belong to this Merge Module" errors for each file.

It seems that this happens because the Language column for the components in the ModuleComponents table is filled with 0 which failes the ICEM05 validation with the ModuleSignature which has Language value 1033

### Expected Result
The module is built successfully and passes ICEM05 validation
