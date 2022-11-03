<div align="center">
AirwayAppiumGaugeTest
</div>

# **SELENIUM //Intelij ///JUNITCore //CUCUMBER // APPIUM
# AllSteps Hepsiburada WithLogin Scenario 
**Tags:Appium**
1. [+] **Uygulamanin acildigi kontrol edilir**
2. [+] **Karsilama Ekrani Skip secenegi ile gecilir**
3. [+] **Seyahat tipi olarak One Way secilir.**
4. [+] **Kalkis havaalani olarak Berlin secilir.**
5. [+] **Varis havaalani olarak Istanbul secilir.**
6. [+] **Arama butonuna tiklanir.**
7. [+] **Ucus secim ekranin geldigi kontrol edilir.**
7. [+] **Rastgele bir ucus secilir.**
7. [+] **Economy Class secenegine tiklanir**


# **Demo
https://user-images.githubusercontent.com/89300182/193265006-5f24a5f4-3a8c-4207-809e-a1769c0666b3.mp4

# pom.xml
 
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/maven-v4_0_0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>org.example</groupId>
    <artifactId>gauge-test</artifactId>
    <version>1.0-SNAPSHOT</version>
    <properties>
        <junit.version>4.13.2</junit.version>
        <gauge.version>0.9.1</gauge.version>
        <log4j.version>1.2.17</log4j.version>
        <appium.version>7.3.0</appium.version>
    </properties>

    <dependencies>
        <dependency>
            <groupId>com.thoughtworks.gauge</groupId>
            <artifactId>gauge-java</artifactId>
            <version>${gauge.version}</version>
            <scope>test</scope>
        </dependency>
        <dependency>
            <groupId>junit</groupId>
            <artifactId>junit</artifactId>
            <version>${junit.version}</version>
            <scope>test</scope>
        </dependency>
        <dependency>
            <groupId>log4j</groupId>
            <artifactId>log4j</artifactId>
            <version>${log4j.version}</version>
        </dependency>
        <dependency>
        <groupId>io.appium</groupId>
        <artifactId>java-client</artifactId>
        <version>${appium.version}</version>
         </dependency>
        <dependency>
            <groupId>org.slf4j</groupId>
            <artifactId>slf4j-api</artifactId>
            <version>1.7.5</version>
        </dependency>
        <dependency>
            <groupId>org.slf4j</groupId>
            <artifactId>slf4j-log4j12</artifactId>
            <version>1.7.5</version>
        </dependency>

    </dependencies>

    <build>
        <plugins>
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-compiler-plugin</artifactId>
                <version>3.7.0</version>
                <configuration>
                    <source>11</source>
                    <target>11</target>
                </configuration>
            </plugin>
            <plugin>
                <groupId>com.thoughtworks.gauge.maven</groupId>
                <artifactId>gauge-maven-plugin</artifactId>
                <version>1.4.3</version>
                <executions>
                    <execution>
                        <phase>test</phase>
                        <configuration>
                            <specsDir>specs</specsDir>
                        </configuration>
                        <goals>
                            <goal>execute</goal>
                        </goals>
                    </execution>
                </executions>
            </plugin>
        </plugins>
    </build>

</project>


 ```

