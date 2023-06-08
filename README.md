[![New Relic Experimental header](https://github.com/newrelic/opensource-website/raw/master/src/images/categories/Experimental.png)](https://opensource.newrelic.com/oss-category/#new-relic-experimental)

# [Reliqstaurants] [build badges go here when available]

> The Reliqstaurants repository was created so that you can test New Relic observability on a small but real project. You don't have to create a special application just to practice, we did it for you. So go ahead and copy the repository, run it locally and try to implement observability for this project yourself. You can find a tip on what the finished project looks like on the "observability" branch

## Getting Started

```
 npm install
 npm run build
```

## Instrumentation
### Account Setup
- You'll need a New Relic account. The good news is that you can create a free account [here](https://newrelic.com/signup) (no credit card required).
### Agent Installation
* Once you've created an account, you can begin installing the agent by first clicking the **Add Data** tab on the left hand navigation pane, as shown below. <img width="1490" alt="Screenshot 2023-06-05 at 2 36 30 PM" src="https://github.com/mchavez-newrelic/relicstaurants/assets/132291725/5fccb01f-e9c4-4877-b977-7df2ff5c2553">
* Search for the Node.js agent in the **Search for any technology** search bar and click the Node.js agent.
* Select **Package manager** for your instrumentation method. <img width="677" alt="Screenshot 2023-06-05 at 2 43 57 PM" src="https://github.com/mchavez-newrelic/relicstaurants/assets/132291725/4eca5c1f-d2fb-4577-a379-2873d383e2f1">
* Follow the steps to instrument your application, starting with giving your application a name. <img width="761" alt="Screenshot 2023-06-05 at 2 33 01 PM" src="https://github.com/mchavez-newrelic/relicstaurants/assets/132291725/c904c018-fbf1-4a53-aab5-2af01e5ca13f">
* Install the APM agent with the command `npm install newrelic --save`.
* Download the `newrelic.js` file and save it in your root project directory.
* Add the New Relic node module into your application
  * Go into your `package.json` and changing the `newstart` script to the following: `node -r newrelic ./server/start.js`. <br/>**OR**<br/>
  * Alternatively, you can navigate to your `/server/start.js` file and add the line `require('newrelic')`
* Start your application by running `npm run newstart`. Application needs to be running in order for the agent to detect it.
* Run the given command in the **Connect your logs and infrastructure step** in your terminal.
* Once you have connected your logs and infrastructure, you may test the connection, as shown below. <img width="724" alt="Screenshot 2023-06-05 at 2 42 09 PM" src="https://github.com/mchavez-newrelic/relicstaurants/assets/132291725/cc634848-c64b-4844-b854-f3a493c4d80f">

### Troubleshooting
* During the step for **Testing the connection**, you may notice that the **On-host logs** fails. This is ok and is most likely due to an unsupported environment.
* You may also run into an issue where the Node.js agent fails to connect, as shown below. If the Node.js agent fails, but you still see data being sent to your New Relic account via the **APM & Services** for Relicstaurants, then you are good to go. If the Node.js agent fails, but you do not see data being sent to your New Relic account, then you may follow the troubleshooting steps [here](https://forum.newrelic.com/s/hubtopic/aAX8W0000008bSdWAI/nodejs-troubleshooting-framework-install). <img width="806" alt="image" src="https://github.com/mchavez-newrelic/relicstaurants/assets/104166698/db0c9529-05a9-4249-927e-6056d52791c2">

## Usage
* Once you've run `npm run build` and `npm run newstart` to start the application, you may navigate to `localhost:3000` in your web browser and see a page as shown below.<img width="1491" alt="Usage_1" src="https://github.com/mchavez-newrelic/relicstaurants/assets/132291725/3e819832-5779-4dcf-bd4b-9ccd1b90d100">
* Simply input an address (does not need to be real), and you will see a page of restaurants as shown below. <img width="1493" alt="Usage_2" src="https://github.com/mchavez-newrelic/relicstaurants/assets/132291725/78de98ea-c7e0-4dee-81d5-760a262a1b8f">
* You may add and place orders as shown below. <img width="1486" alt="Usage_3" src="https://github.com/mchavez-newrelic/relicstaurants/assets/132291725/d5b7d486-76b0-4db8-9df2-a3d174d06668">

## Building
> Because backend of app is already in repository we need to build it manually and then make newstart, that commands will at first build whole application with backend and next will serve it in browser.

## Support

New Relic hosts and moderates an online forum where customers can interact with New Relic employees as well as other customers to get help and share best practices. Like all official New Relic open source projects, there's a related Community topic in the New Relic Explorers Hub. You can find this project's topic/threads here:

> Add the url for the support thread here

## Contributing

We encourage your contributions to improve [project name]! Keep in mind when you submit your pull request, you'll need to sign the CLA via the click-through using CLA-Assistant. You only have to sign the CLA one time per project.
If you have any questions, or to execute our corporate CLA, required if your contribution is on behalf of a company, please drop us an email at opensource@newrelic.com.

**A note about vulnerabilities**

As noted in our [security policy](../../security/policy), New Relic is committed to the privacy and security of our customers and their data. We believe that providing coordinated disclosure by security researchers and engaging with the security community are important means to achieve our security goals.

If you believe you have found a security vulnerability in this project or any of New Relic's products or websites, we welcome and greatly appreciate you reporting it to New Relic through [HackerOne](https://hackerone.com/newrelic).

## License

[Project Name] is licensed under the [Apache 2.0](http://apache.org/licenses/LICENSE-2.0.txt) License.

> [If applicable: The [project name] also uses source code from third-party libraries. You can find full details on which libraries are used and the terms under which they are licensed in the third-party notices document.]

```

```
