FROM dart:stable as builder
COPY . /dart-server
WORKDIR /dart-server
RUN dart compile exe ./bin/dart_server.dart -o ./build/dartserve

FROM debian:buster-slim
COPY --from=builder /dart-server/build /bin
CMD ["dartserve"]
