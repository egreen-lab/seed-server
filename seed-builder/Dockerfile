FROM java:8-jdk
# Install Gradle
RUN groupadd -r gradle && useradd -r -g gradle gradle

RUN wget https://services.gradle.org/distributions/gradle-2.4-all.zip
RUN unzip gradle-2.4-all.zip
RUN mv gradle-2.4 /opt/
RUN rm gradle-2.4-all.zip

# Environment variables
ENV GRADLE_HOME /opt/gradle-2.4
ENV PATH $PATH:$GRADLE_HOME/bin


ENV WORK_BASE /opt/workspace
RUN mkdir -p "$WORK_BASE" && chown gradle:gradle "$WORK_BASE"
WORKDIR $WORK_BASE
