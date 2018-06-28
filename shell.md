## java

```
sudo vim ~/.bashrc
```

export ANDROID_HOME=~/Android/Sdk

export JAVA_HOME=/usr/local/jdk1.8.0_162

export JRE_HOME=${JAVA_HOME}/jre

export CLASSPATH=.:%{JAVA_HOME}/lib:%{JRE_HOME}/lib

export PATH=${JAVA_HOME}/bin:${JRE_HOME}/bin:${ANDROID_HOME}/tools:${ANDROID_HOME}/platform-tools:${PATH}

source ~/.bashrc

## android studio

avdmanager create avd -n test -k "system-images;android-25;google_apis;x86"

avdmanager delete avd -n name

avdmanager list avd

## nvm:Node

## react-native-cli

## watchman

sudo apt-get install autoconf automake python-dev

git clone https://github.com/facebook/watchman.git cd watchman git checkout v4.7.0 # 这是facebook官方文档说的最新稳定版本 ./autogen.sh ./configure make sudo make install

vim /etc/sysctl.conf

fs.inotify.max_user_watches=524288

/sbin/sysctl -p

/proc/sys/fs/inotify/max_user_watches

## 进入 Android/Sdk/tools 目录，执行emulator -avd Nexus_5X_API_24

https://reactnative.cn/docs/0.51/getting-started.html

https://developer.android.com/studio/command-line/avdmanager.html