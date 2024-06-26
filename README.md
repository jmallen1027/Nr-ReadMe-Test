# nr1-field-viz

## About this Nerdpack

This application addresses a common issue faced by users when creating dashboard charts: query timeouts due to long-running queries. By using this app, users can ensure that their dashboard panels populate efficiently and reliably, avoiding the frustration of unresponsive or incomplete data visualizations.

### Key features include:

Seamless integration: Provides an experience similar to what you enjoy in New Relic, making it easy for you to create and manage dashboard panels.

Efficient data handling: Optimizes query performance to prevent timeouts, ensuring that all charts and data visualizations load correctly and promptly.

Flexible query management: Helps you handle long-running queries effectively, breaking them down into manageable parts to ensure complete data retrieval without performance issues.

With this app, you can build comprehensive and responsive dashboards. You can also maintain the quality and reliability of your data visualizations even with complex and extensive queries.

![Screenshot #1](/screenshot_01.png)
![Screenshot #2](/screenshot_02.png)
![Screenshot #1](/screenshot_01.png)

## Open source license

This project is distributed under the [Apache 2 license](LICENSE).

## What do you need to make this work?

Required:

- New Relic Account
- Must be a full or core user in order to use and visualize NR1 Nerdpacks

Good to have:

- Experience with New Relic NRQL
- Experience with the NR1 CLI

Resources 

- [New Relic University](https://learn.newrelic.com/) 
- [New Relic NRQL Docs](https://docs.newrelic.com/docs/nrql/get-started/introduction-nrql-new-relics-query-language/)
- [New Relic Developers](https://developer.newrelic.com/build-apps/)

## Getting started

Complete the following to run the NerdPack locally:

1. Ensure that you have [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and [NPM](https://www.npmjs.com/get-npm) installed.
    * If you're unsure whether you have one or both of them installed, run the following commands.
    * If you have them installed, these commands return a version number; if not, the commands aren't recognized.
      ```bash
      git --version
      npm -v
      ```
2. Install the [NR1 CLI](https://one.newrelic.com/launcher/developer-center.launcher) by going to [the developer center](https://one.newrelic.com/launcher/developer-center.launcher) and following the instructions to install and set up your New Relic development environment. This should take about five minutes.
3. Execute the following command to clone this repository and run the code locally against your New Relic data:

    ```bash
    nr1 nerdpack:clone -r https://github.com/newrelic/nr1-field-viz.git
    cd /nr1-field-viz/visualizations
    nr1 nerdpack:serve
    ```

Visit [https://one.newrelic.com/?nerdpacks=local](https://one.newrelic.com/?nerdpacks=local) to launch your app locally. 

## Deploying this Nerdpack

Open a command prompt in the app's directory (`/nr1-field-viz/visualizations`) and run the following commands, replacing the placeholders with your information:

```bash
# If you need to create a new uuid for the account to which you're deploying this app, uncomment the next line and run it:
# nr1 nerdpack:uuid -g [--profile=your_profile_name]
# To see a list of APIkeys / profiles available in your development environment, run nr1 credentials:list
nr1 nerdpack:publish [--profile=your_profile_name]
nr1 nerdpack:deploy [-c [DEV|BETA|STABLE]] [--profile=your_profile_name]
nr1 nerdpack:subscribe [-c [DEV|BETA|STABLE]] [--profile=your_profile_name]
```
## Using this Nerdpack
- Visit [https://one.newrelic.com](https://one.newrelic.com), and launch your app in New Relic.
- Enter values for the chart name, account ID, query, and then select a chart type.
- Do not include any time ranges when entering the query. The nerdpack will update query when the time range is changed. 
- Add to dashboard.
- Test different time ranges. 

# Support

New Relic has open-sourced this project. This project is provided AS-IS WITHOUT WARRANTY OR DEDICATED SUPPORT. Issues and contributions should be reported to the project here on GitHub.

We encourage you to bring your experiences and questions to the [Explorers Hub](https://discuss.newrelic.com) where our community members collaborate on solutions and new ideas.

## Community

New Relic hosts and moderates an online forum where customers can interact with New Relic employees as well as other customers to get help and share best practices. Like all official New Relic open source projects, there's a related Community topic in the New Relic Explorers Hub. You can find this project's topic/threads here:

https://discuss.newrelic.com/t/nr1-field-viz (Note that this URL is subject to change before GA)

## Issues / enhancement requests

Issues and enhancement requests can be submitted in the [Issues tab of this repository](../../issues). Please search for and review the existing open issues before submitting a new issue.

# Contributing

Contributions are encouraged! If you submit an enhancement request, we'll invite you to contribute the change yourself. Please review our [Contributors Guide](CONTRIBUTING.md).

Keep in mind that when you submit your pull request, you'll need to sign the CLA via the click-through using CLA-Assistant. If you'd like to execute our corporate CLA, or if you have any questions, please drop us an email at opensource+nr1-field-viz@newrelic.com.
