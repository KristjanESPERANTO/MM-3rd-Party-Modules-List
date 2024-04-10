# 3rd Party Modules for MagicMirror²

Transition from Wiki List to this repo.

## Current situation

The list of MagicMirror 3rd-party modules is currently maintained in a wiki. This is prone to errors, as not every user is thorough in formatting and there is no automatic syntactic or content check.

## Proposed solution

The idea is to replace this with a new GitHub repository. This repository will either contain one large file or multiple files per category. The format is also not yet clear, possibly YAML or JSON. YAML would have the advantage of having simpler syntax.

### Adding new modules

To add a new module, a pull request (PR) would have to be created. Automatic checks could be run on the PR, and if these are successful, the PR would be automatically accepted.

### Advantages

* Reduced error rate: Automatic checks would ensure that all modules are formatted correctly and meet certain quality standards.
* Simplified maintenance: The use of a GitHub repository would make it easier to maintain the list and track changes.
* Improved usability: The list would be easier to use for both developers and users.

### Target groups

* Module developers: The new system would make it easier for developers to add and update their modules.
* Projects: Projects that use the list, such as mmpm, MMM-Remote-Control and [MagicMirror-3rd-Party-Modules](https://kristjanesperanto.github.io/MagicMirror-3rd-Party-Modules/), would be able to access the data more easily.
* Simple users: The list would be easier to use for users who are not familiar with GitHub.
* Repository maintainers: The new system would make it easier for maintainers to keep the list up-to-date.
* MagicMirror community: The community would benefit from a more comprehensive and reliable list of modules.

### Next steps

* Choose a format: Decide whether to use YAML or JSON as the file format for the list.
* Implement automatic checks: Set up automatic checks to ensure that PRs are formatted correctly and meet certain quality standards.
* Transform the input format in several output formats (JSON, Markdown, ...)
* Integrate the solution into the projects mentioned obove.
* Write How-Tos.
* Move the repository to the official MagicMirror project.
* Replace the list in the wiki by a link to this new repository.

### Open questions

* Which format is best suited for the list? YAML and JSON are both viable options, but each has its own advantages and disadvantages. Should we consider other formats?
* Create a separate file for each category?

### Conclusion

The proposed solution would improve the situation of the MagicMirror 3rd-Party Module List in several ways. It would reduce the error rate, simplify maintenance, improve usability, and increase visibility. The next steps are to choose a format, set up the repository, implement automatic checks, and promote the repository.

### Format draft

YAML:

```yaml
- name: MMM-01ZM
  category: Utility / IOT / 3rd Party / Integration
  url: https://github.com/rubinho101/MMM-01ZM
  id: rubinho101/MMM-01ZM
  maintainer: rubinho101
  description: Display Xiaomi LYWSDCGQ 01ZM Temperature and Humidity sensor values directly AND Nova SDS011 PM Air Quality sensor data.
  last-mm-version-tested-with: 2.27.0

- name: MMM-1-Second-A-Day
  category: Entertainment / Misc
  url: https://github.com/GaryLChew/MMM-1-Second-A-Day
  id: GaryLChew/MMM-1-Second-A-Day
  maintainer: GaryLChew
  description: Record daily 1-second-clips and automatically generate a 1-second-a-day video of your life.

- name: MMM-2Day-NOAA-Forecast
  category: Weather
  url: https://github.com/jinserk/MMM-2Day-NOAA-Forecast
  id: jinserk/MMM-2Day-NOAA-Forecast
  maintainer: jinserk
  description: Show 4 consecutive 12-hr forecast, provided by <a target="_blank" href="https://www.weather.gov/documentation/services-web-api">NOAA National Weather Service API</a>. No user registration nor API-key required.
```
