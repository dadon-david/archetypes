# My archetypes
This repo contains some archetypes I created to start a project quickly

## Archetypes in this repository

### backend-archetype

#### Description
This is a maven archetype to create a java backend to be deployed on a servlet container. It contains, among other:
* A `.gitignore` and a `README.md`
* A ready to use `pom.xml` with Jersey and Swagger
* A Web Application Deployment Descriptor `web.xml`

#### Prerequisite
* JDK 1.8+
* Maven 3.6.3+

#### Installation
```zsh
% cd backend-archetype
% mvn install
```

#### Use the archetype
On the location where you want the directory to be created:
* Replace the fields enclosed by curly braces `{}` with the values you want (Don't include the curly braces)
* For the java version, you can use `1.8` for example
* Run the maven command

```zsh
mvn archetype:generate \
-DarchetypeGroupId=sh.david \
-DarchetypeArtifactId=backend-archetype \
-DarchetypeVersion=1.0-SNAPSHOT \
-DarchetypeCatalog=local \
-DgroupId={AddYourGroupId} \
-DartifactId={AddYourArtifactId}\
-Dpackage={AddYourPackageName} \
-DjavaVersion={AddYourJavaVersion} \
-DgithubUsername={AddYourGithubUserName} \
-DinteractiveMode=false
```

## License
```
Copyright 2020 David Dadon

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```