# coldfusion-docker-starter
Adobe ColdFusion development with Docker starter project

## What is this?
This repo exists to make your life easier when starting a new Adobe ColdFusion project or converting an existing ColdFusion project to run inside a Docker container.

## How do I use it?
### Prerequisites
The only prerequisite that you need to use this repo is to have Docker installed. You can install Docker Desktop on Mac or Windows. If you are on Windows, I **highly** recommend setting up Windows Subsystem for Linux (WSL) and using it for your development environment.

### Usage
* Download the zip file from GitHub and extract it to a folder.
* In the folder where you extracted the zip file, run the following command in a terminal window `docker-compose up`
* In your browser, browse to `https://localhost:8500`
* Add your application code in the `app/` folder located in the directory where you extracted the repo
* View the ColdFusion logs under `logs/` for execptions and other log information you need while developing

*Notes*
* If you're on Mac or Linux (including WSL), you'll need to run the `fixperms.sh` file in the root of the repo to set the permissions on the `logs/` folder correctly so that ColdFusion can create its log files there.
* If you need a specific version of ColdFusion, you can specify a particular tag on line 5 of `docker-compose.yml`. You can find a complete list of tags for the image [here](https://bintray.com/eaps/coldfusion/cf%3Acoldfusion)

## Contributing
I'd love to hear from you on what else you would like to see in this starter project. Please create an issue on the repo or clone the repo and submit a PR with your proposed changes.
