# Flagship Flag Reference Action

This action synchronize Flagship flag references in your codebase to the Flagship Platform.

## Inputs

### `flagshipToken`

**Required** The API Token for the Flagship Platform. You can create one in the Platform Integration settings of the Flagship Platform.

### `flagshipEnvId`

**Required** The Environment ID in the Flagship Platform. You can get it from the Settings / API & Settings menu on the Flagship Platform.

### `repositoryUrl`

**Required** The URL of the repository URL you will be scanning. You can use Github environment variables such as `GITHUB_SERVER_URL` and `GITHUB_REPOSITORY` to fill this out.

### `repositoryBranch`

**Required** The branch of the repository you will be scanning. You can use Github environment variables such as `GITHUB_REF` to fill this out.

### `directory`

**optional** The directory of the subfolder of the repository you will be scanning. Default: `.`

### `filesToExclude`

**optional** comma separated glob patterns that your want to exclude from the analysis. Default: '.git'