# gitlab_actions_testing

This repository was created to experiment with GitHub Actions.

## Steps

1. **Set up the repository**: Clone it locally onto your PC.

2. **Create a new branch**: Add a file named `gitleaks.yml` in the `.github/workflows` directory.

3. **Refer to Gitleaks documentation**:  
   Visit the [Gitleaks repository](https://github.com/gitleaks/gitleaks?tab=readme-ov-file) and refer to the [GitHub Action documentation](https://github.com/gitleaks/gitleaks-action).

4. **Update and push `gitleaks.yml`**:  
   Add the necessary content to the `gitleaks.yml` file, push it to the GitHub repository, and create both a merge request and a pull request.

5. **Create a `passwords.txt` file**:  
   Add multiple secrets, such as passwords, API keys, and tokens.

6. **Verify secret detection**:  
   Push the `gitleaks.yml` file to the GitHub repository, then check the GitHub Action to see if it detects the secrets.

## Note

I encountered an issue with permissions while setting up the GitHub Action for secret scanning. To resolve this, it was necessary to change the workflow permissions:

1. Go to **Settings** → **Actions** → **General**.
2. Change **Workflow permissions** to "Read and write permissions."

For the sake of this project, this change was sufficient. However, it is possible to specify more granular permissions in the workflow using YAML.
