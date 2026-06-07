# Simple Spring Boot Test Application using Keycloak as IdP

## Usage

1. Install required packages:

```shell
sudo apt-get -y install maven openjdk-25-jre-headless
```

2. In your Keycloak realm of choice, create an OIDC client

3. Edit [application.properties](src/main/resources/application.properties)
   - In `spring.security.oauth2.client.provider.external`, modify `issuer-uri`, `client-name`, `client-id` and `client-secret`.

4. Build and run the test application:

```shell
mvn clean spring-boot:run
```

## Author, Copyright and License Information

*Note:* The code in this example is heavily based on Muhammad Edwin's blog
article "How to integrate Spring Boot 3, Spring Security, and Keycloak" and the
accompanying GIT repository:

* <https://developers.redhat.com/articles/2023/07/24/how-integrate-spring-boot-3-spring-security-and-keycloak>
* <https://github.com/edwin/spring-3-keycloak>

Licensed under the Apache License, Version 2.0 (the "License"); you may not use
this file except in compliance with the License. You may obtain a copy of the
License at <http://www.apache.org/licenses/LICENSE-2.0>

Unless required by applicable law or agreed to in writing, software distributed
under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
CONDITIONS OF ANY KIND, either express or implied. See the License for the
specific language governing permissions and limitations under the License.
