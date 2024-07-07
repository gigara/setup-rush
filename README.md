# Setup Rush GitHub Action

This GitHub Action sets up Rush with caching support for your workflows. It allows you to configure and cache pnpm and Rush directories, set environment variables, and run Rush commands.

## Inputs

### `pnpm`
**Description:** (Optional) Specify the PNPM version to use. Will not install if not provided.  

### `node`
**Description:** (Optional) Specify the Node.js version to use. Will not install if not provided.  

### `cache-rush`
**Description:** (Optional) Boolean to enable caching of Rush directories. Default is true.  
**Default:** `'true'`

### `cache-rush-dir`
**Description:** (Optional) Directories to cache with Rush cache key. Default includes common/temp/install-run and ~/.rush.  
**Default:** 
  - `common/temp/install-run`
  - `~/.rush`

### `cache-pnpm`
**Description:** (Optional) Boolean to enable caching of PNPM directories. Default is true.  
**Default:** `'true'`

### `cache-pnpm-dir`
**Description:** (Optional) Directories to cache with PNPM cache key. Default includes common/temp/pnpm-store and ~/.cache/Cypress.  
**Default:** 
  - `common/temp/pnpm-store`
  - `~/.cache/Cypress`

### `set-env`
**Description:** (Optional) Boolean to set ACTIONS_CACHE_URL & ACTIONS_RUNTIME_TOKEN envs. You may need to enable this if you are using [rush-github-action-build-cache-plugin](rush-github-action-build-cache-plugin) in your project.  
**Default:** `'true'`

### `rush-install`
**Description:** (Optional) Run rush install command.  
**Default:** `'true'`

### `rush-build`
**Description:** (Optional) Run rush build command.  
**Default:** `'false'`

### `optional-build-args`
**Description:** (Optional) Additional arguments for rush build command.  
**Default:** `''`


