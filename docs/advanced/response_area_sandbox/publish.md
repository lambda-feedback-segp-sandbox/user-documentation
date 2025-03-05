# Response Area Packages

Response area types developed outside of `client-web` depend on the following
packages built from within the repository:

- `packages/styles/`

    Exposes the Material UI theme used throughout the frontend so that new
    response area types have consistent user interfaces.

- `packages/response-area-api/`

    Exposes the GraphQL interface types used by response areas for communication
    with the backend.

- `packages/response-area-base/`

    Exposes the `ResponseAreaTub` base class. All response area types include a
    subclass of this class to specify their input and wizard components.

Changes made to files in these directories will be visible from the main
application immediately, but new versions will eventually need to be published
to make them available to externally developed response areas.

## Publish a New Version

1. **Update the `version` field of the package's `package.json`**

    Version bumps should follow the [Semantic Versioning](https://semver.org)
    standard.

    The versions of the packages are independent, so you only need to bump the
    version of the package(s) you have updated.

    You will need to push the change to the `main` branch on GitHub, either as a
    standalone commit or as part of a Pull Request.

1. **Run the GitHub Actions workflow**

    1. Go to the **Actions** tab for the `client-web` repository on GitHub.

    1. Click **Publish a package to GitHub Packages** in the left column.

    1. Open the **Run workflow** dropdown on the right, select the package
       you have updated, and start the workflow.

    When the workflow has finished, your new version will be accessible from the
    GitHub Packages registry.

Attempting to publish a package under a version which has previously been
published will cause the GitHub Actions workflow to fail.
