# Aplicaci�n del Administrador
[![Build Status](https://travis-ci.org/sitmun/sitmun-admin-app.svg?branch=master)](https://travis-ci.org/sitmun/sitmun-admin-app)
[![Quality Gate](https://sonarcloud.io/api/badges/gate?key=sitmun-admin-app)](https://sonarcloud.io/dashboard?id=sitmun-admin-app)

# Build and run (local)
Clone the repository.

Build: `$ ./build-scripts/build-local.sh`. If the build is successful it will launch a SonarQube analysis in SonarCloud. This requires that you have a SonarCloud user added to the SITMUN organization, and a token. To create a token, go to your SonarCloud account page, Security tab, and generate one. Then create a file in `$HOME/.gradle/gradle.properties` with this line: `systemProp.sonar.login=LONG_CHAR_STRING_THAT_IS_YOUR_SONARCLOUD_TOKEN`. If you already had that file, simply add the line to it.

Run: `$ ./gradlew bootRun` and go to <http://localhost:8080>.

If you the SonarCloud analysis has been properly run, you can see the report by clicking on the quality gate badge above.

# Dependencies
This project depends on these plugins (already considered in the build script):

- [sitmun-plugin-core](https://github.com/sitmun/sitmun-plugin-core)
