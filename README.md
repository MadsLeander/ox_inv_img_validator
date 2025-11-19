# About

ox_inv_img_validator is a utility script to list missing and remove unused item images from [ox_inventory](https://github.com/CommunityOx/ox_inventory). This is most useful for server developers who want to mass remove unused images, as well as figure out what items are lacking images.    

This resource is only intended to be used in a development environment, not production.

# Installation

This is a drag and drop resource.

1. Add the `ox_inv_img_validator` resource to your resources folder.
2. Type `ensure ox_inv_img_validator` into your server console (you might need to type `refresh` first if you added it while the server was active).
3. Done!

# Usage

## Item image check/list
Use the `validate_inventory_images` command in the server console to list all missing and unused item images.

## Removing unused files
Use the `cleanup_inventory_images` command in the server console to remove all unused item images.

## Configuration

You can add ignored files and items by adding them inside the `IGNORE_UNUSED_IMAGES` and `IGNORE_MISSING_IMAGES` tables respectively (located at the top of server.lua).  

If you have changed the name of ox_inventory you will have to change the `OX_INVENTORY_RESOURCE_NAME` variable in server.lua to match the resource name. The script will then automatically find the path to the item images.

## Contributions

Contributions are welcome. If you find a bug or see a need for an improvement, please add an issue or open a PR!
