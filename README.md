openpilot
openpilot is an operating system for robotics.
Currently, it upgrades the driver assistance system in 275+ supported cars.

Docs · Roadmap · Contribute · Community · Try it on a comma 3X
Quick start: bash <(curl -fsSL openpilot.comma.ai)

openpilot tests codecov License: MIT X Follow Discord

		
Using openpilot in a car
To use openpilot in a car, you need four things:

Supported Device: a comma 3/3X, available at comma.ai/shop.
Software: The setup procedure for the comma 3/3X allows users to enter a URL for custom software. Use the URL openpilot.comma.ai to install the release version.
Supported Car: Ensure that you have one of the 275+ supported cars.
Car Harness: You will also need a car harness to connect your comma 3/3X to your car.
We have detailed instructions for how to install the harness and device in a car. Note that it's possible to run openpilot on other hardware, although it's not plug-and-play.

Branches
branch	URL	description
release3	openpilot.comma.ai	This is openpilot's release branch.
release3-staging	openpilot-test.comma.ai	This is the staging branch for releases. Use it to get new releases slightly early.
nightly	openpilot-nightly.comma.ai	This is the bleeding edge development branch. Do not expect this to be stable.
nightly-dev	installer.comma.ai/commaai/nightly-dev	Same as nightly, but includes experimental development features for some cars.
To start developing openpilot
openpilot is developed by comma and by users like you. We welcome both pull requests and issues on GitHub.

Join the community Discord
Check out the contributing docs
Check out the openpilot tools
Read about the development workflow
Code documentation lives at https://docs.comma.ai
Information about running openpilot lives on the community wiki
Want to get paid to work on openpilot? comma is hiring and offers lots of bounties for external contributors.

Safety and Testing
openpilot observes ISO26262 guidelines, see SAFETY.md for more details.
openpilot has software-in-the-loop tests that run on every commit.
The code enforcing the safety model lives in panda and is written in C, see code rigor for more details.
panda has software-in-the-loop safety tests.
Internally, we have a hardware-in-the-loop Jenkins test suite that builds and unit tests the various processes.
panda has additional hardware-in-the-loop tests.
We run the latest openpilot in a testing closet containing 10 comma devices continuously replaying routes.
Licensing
openpilot is released under the MIT license. Some parts of the software are released under other licenses as specified.

Any user of this software shall indemnify and hold harmless Comma.ai, Inc. and its directors, officers, employees, agents, stockholders, affiliates, subcontractors and customers from and against all allegations, claims, actions, suits, demands, damages, liabilities, obligations, losses, settlements, judgments, costs and expenses (including without limitation attorneys’ fees and costs) which arise out of, relate to or result from any use of this software by user.

THIS IS ALPHA QUALITY SOFTWARE FOR RESEARCH PURPOSES ONLY. THIS IS NOT A PRODUCT. YOU ARE RESPONSIBLE FOR COMPLYING WITH LOCAL LAWS AND REGULATIONS. NO WARRANTY EXPRESSED OR IMPLIED.

User Data and comma Account
By default, openpilot uploads the driving data to our servers. You can also access your data through comma connect. We use your data to train better models and improve openpilot for everyone.

openpilot is open source software: the user is free to disable data collection if they wish to do so.

openpilot logs the road-facing cameras, CAN, GPS, IMU, magnetometer, thermal sensors, crashes, and operating system logs. The driver-facing camera is only logged if you explicitly opt-in in settings. The microphone is not recorded.

By using openpilot, you agree to our Privacy Policy. You understand that use of this software or its related services will generate certain types of user data, which may be logged and stored at the sole discretion of comma. By accepting this agreement, you grant an irrevocable, perpetual, worldwide right to comma for the use of this data.
