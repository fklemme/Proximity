# Proximity
A tool to assemble Magic: The Gathering proxies from a set of template images

# Build 

Using Ubuntu 20.04:

    sudo apt install openjdk-16-jdk
    chmod +x gradlew
    ./gradlew shadowJar
    
    printf "1x Storm Crow\n1x Forest\n" > decklist.txt
    cd run
    java -jar ../build/libs/proximity*-all.jar --cards=../decklist.txt --template=normal

A note for myself:

    --override=set:xlcu
