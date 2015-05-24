FROM java:8-jdk
# Install Gradle
RUN wget https://services.gradle.org/distributions/gradle-2.4-all.zip
RUN unzip gradle-2.4-all.zip
RUN mv gradle-2.4 /opt/
RUN rm gradle-2.4-all.zip

# Environment variables
ENV GRADLE_HOME /opt/gradle-2.4
ENV PATH $PATH:$GRADLE_HOME/bin

