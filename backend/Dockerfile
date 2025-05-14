FROM eclipse-temurin:21-jdk-jammy

WORKDIR /app

COPY . .

# 依存関係インストールとビルド
RUN ./gradlew build --no-daemon

EXPOSE 8080

CMD ["./gradlew", "bootRun"]