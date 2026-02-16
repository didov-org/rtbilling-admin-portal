# RTBilling Admin Portal

This project is a fork of [UniBee Admin Portal](https://github.com/UniBee-Billing/unibee-admin-portal), a single-page web application serving as the front-end for the UniBee billing admin management system. This fork has been modified since February 2025.

## Changes from upstream

This fork includes modifications to the original UniBee Admin Portal. Key changes include enhancements to subscription usage metrics, metering usage actions, and addon plan calculations. For a full list of changes, see the [commit history](https://github.com/bdidov/rtbilling-admin-portal/commits/main).

## Prerequisites

- Node.js 18+

## Getting started

Clone this repository and install the dependencies.

```shell
# Clone this repository
git clone https://github.com/bdidov/rtbilling-admin-portal

# Install dependencies
cd rtbilling-admin-portal
yarn install
```

### Running the application

Define the following env variables in `.env` file.

```
VITE_API_URL=http://unibee.top/unib
VITE_STRIPE_PUBLIC_KEY=YOUR_STRIPE_PUBLIC_KEY
```

> .env.local for development, .env.production for production build

Now you can start dev server using the following command.

```shell
yarn dev
```

### Building the application

To build the application, run the following command:

```shell
yarn build
```

The build command will generate the static files in the `dist` folder of the project.

### Building with Docker

The admin portal also supports building the application using Docker, run the following command to build the docker image:

```shell
docker build -t <tag> .
```

## Development

Use `yarn add <package>` to add a new dependency, don't use `npm install <package>`. Create your own local branch for development, then create a PR to merge into the develop branch.

## License

This project is licensed under the [GNU Affero General Public License v3.0](LICENSE) (AGPLv3), the same license as the original [UniBee Admin Portal](https://github.com/UniBee-Billing/unibee-admin-portal).

This is a modified version of the original program. In accordance with AGPLv3 Section 5, this modified version is distributed under the same license terms. See the [LICENSE](LICENSE) file for full details.
