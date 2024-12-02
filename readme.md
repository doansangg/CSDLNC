# Sửa lỗi lombok
* lombok đang bị lỗi backend

### vào ổ C: tìm thư mục: C:\Users\doans\\.m2\repository\org\projectlombok\lombok\1.18.24( lưu ý chỗ version này lấy version cao hơn ).
* Chạy lệnh: ```java -jar lombok-1.18.24.jar```
* :Làm theo video này: link: "https://mega.nz/folder/GqJnFD5I#oS3oG-exI2LKvCuHW_Q0Og" 
* đều chạy đưuọc trên mysql workbend hoặc xampp

* ### chạy trên ubuntu
* cài java11, default trên ubutu 22.04 và maven
```
Apache Maven 3.9.9 (8e8579a9e76f7d015ee5ec7bfcdc97d260186937)
Maven home: /opt/maven
Java version: 11.0.25, vendor: Ubuntu, runtime: /usr/lib/jvm/java-11-openjdk-amd64
Default locale: en_US, platform encoding: UTF-8
OS name: "linux", version: "6.8.0-49-generic", arch: "amd64", family: "unix"
```
* Thêm phần 
```
		<dependency>
			<groupId>org.projectlombok</groupId>
			<artifactId>lombok</artifactId>
			<version>1.18.24</version> <!-- Sử dụng phiên bản mới nhất -->
			<scope>provided</scope>
		</dependency>
```
vào trong pom.xml
* Chạy lệnh ```mvn clean install``` , sau đó khi build xong, trong thư mục tagert có file .jar. Tiếp tục chạy ```java -jar target/your-project-name.jar``` để start server
* nodejs version 16.20.2
* npm install -g @angular/cli@16.2.10
