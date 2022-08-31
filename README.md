# Flagship Flag Reference Action

This action synchronize Flagship flag references in your codebase to the Flagship Platform.
It uses the Codebase Analyzer provided by Flagship to look for flag usage in your codebase and send line numbers, context and file URL to Flagship, in order to match a flag in the platform to its usage in the code.

More information here: [Codebase Analyzer](https://docs.developers.flagship.io/docs/codebase-analyzer)

## Inputs

### `flagshipClientId`

**Required** The API Client ID for the Flagship Remote Control API. You can create one in the Settings / Integration settings of the Flagship Platform.

### `flagshipClientSecret`

**Required** The API Client Secret for the Flagship Remote Control API. You can create one in the Settings / Integration settings of the Flagship Platform.

### `flagshipEnvId`

**Required** The Environment ID in the Flagship Platform. You can get it from the Settings / API & Settings menu on the Flagship Platform.

### `flagshipAccountId`

**Required** The Account ID in the Flagship Platform. You can get it from the Settings / Account menu on the Flagship Platform.

### `repositoryUrl`

**Required** The URL of the repository URL you will be scanning. You can use Github environment variables such as `GITHUB_SERVER_URL` and `GITHUB_REPOSITORY` to fill this out.

### `repositoryBranch`

**Required** The branch of the repository you will be scanning. You can use Github environment variables such as `GITHUB_REF` to fill this out.

### `directory`

**optional** The directory of the subfolder of the repository you will be scanning. Default: `.`

### `filesToExclude`

**optional** comma separated glob patterns that your want to exclude from the analysis. Default: '.git'
