# Bombcampaign

A sigal Java application writen Clojure for sending mask email for your general purpose.
This application using [Postal](https://github.com/drewr/postal) is a library for constructing and sending RFC822-compliant Internet email messages. and [clojure.data.csv](https://github.com/clojure/data.csv) A CSV reader/writer to/from Clojure data structures to interact with data.

## Usage
### I Build
If you want to contribute or build on your won pc here is the environment setup [How to install Leiningen project tool for Clojure on Arch Linux](https://www.ayoungnotes.com/How-to-install-Leiningen-project-tool-for-Clojure-on-Arch-Linux).

Bellow is the build guide:

1) Download the dependencies with the following commend: 
```
lein deps
```
2) Compile Application with the following commend: 
```
lein compile
```
3) Build a Java Application with the following commend: 
```
lein uberjar
```
4) Run Application
```
java -jar bombcampaign-0.1.0-SNAPSHOT-standalone.jar
```

### Start Sending Email

There are three files in side data folder. config.csv is where you confige SMTP server. In contact.csv is list of email who you want to send your email to. And content.csv is your email body.

Note* 
- Make sure that the data directory is there with bombcampaign-0.1.0-SNAPSHOT-standalone.jar
- To verify the sending email and error log go to data/sendmaillog/mailinglog.log

## License

Copyright © 2020 Mr.Ayoung

Distributed under Free License.
