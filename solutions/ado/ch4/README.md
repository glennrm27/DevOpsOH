# Challenge 4

All pipelines are implemented in the `.azure-pipelines` folder. There are four pipelines for each API: *POI*, *Trips*, *UserJava*, and *User*

On the first run, you might be asked to permit access to variable group and service connection. Also, if the pipeline gets stuck in Pending state, check if the lacking permissions are not blocking it.

![ado-ch3-permission1](..\ch3\ado-ch3-permission1.png)

![ado-ch3-permission2](..\ch3\ado-ch3-permission2.png)

## Challenge

A *pull request* workflow needs to be built, which builds API,unit tests the API, and publishes test results. It is triggered by pull request creation.

The solution is split into four files for each API.

Follow the same validation steps as <a href="../ch3/README.md" target="_blank">Challenge 3</a>
