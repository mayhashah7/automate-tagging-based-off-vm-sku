# automate-tagging-based-off-vm-sku
The custom Azure Policy policy “Tag Based on VM SKU” will identify all VMs with a specified SKU (vmSKU). All VMs with this SKU will then be given a specified tag name (tagName) and tag value (tagValue). Since this is a policy with a “modify” effect we can remediate existing resources. Newly created VMs with the specified SKU will automatically have the tag added. If you would like to have the same tag added to a few different VM SKUs, you can change the vmSKU parameter to accept an array instead of a single string.
