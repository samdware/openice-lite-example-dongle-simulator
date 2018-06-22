## OpenICE-lite Example: Dongle Simulator

[![Build Status](https://travis-ci.org/samdware/openice-lite-example-dongle-simulator.svg?branch=master)](https://travis-ci.org/samdware/openice-lite-example-dongle-simulator)

This repository provides an example of using the [OpenICE-lite Core](https://github.com/samdware/openice-lite) to simulate a synthetic medical device data stream through the MQTT broker.

### Requirements
In order to run the simulator, you need:
- Java 1.8 installed
- MQTT Broker credential

### Configuration
You can configure the simulator via the included `sim.properties` file. Detailed options can be referred from OpenICE-lite Core API documentation. These are some basic options:
- `project_name`: default root for the MQTT topic
- `broker`: MQTT broker address (in the form of `tcp://address:port`, separated by commas if using a broker cluster)
- `username`: (optional) user name to login to the MQTT broker
- `password`: (optional) password to login to the MQTT broker
- `data`: sample data to be sent

### How to use
To run the simulator, execute the following commands:
- On Unix system
```
./gradlew run
```
- On Windows system
```
gradlew.bat run
```

### DISCLAIMER
USE OF THIS SOFTWARE IN ANY WAY AND RELIANCE ON THE CONTENTS IS DONE AT THE USER'S DISCRETION AND RISK. YOU HEREBY AGREE THAT YOU WILL BE SOLELY RESPONSIBLE FOR ANY DAMAGE OR HARM THAT RESULTS FROM SUCH USE. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.