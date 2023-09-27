FROM debezium/server:nightly

ARG OTEL_VERSION=1.30.1

RUN set -eux; \
    curl -sSL -o lib/quarkus-opentelemetry-3.4.1.jar https://repo1.maven.org/maven2/io/quarkus/quarkus-opentelemetry/3.4.1/quarkus-opentelemetry-3.4.1.jar; \
    curl -sSL -o lib/opentelemetry-javaagent.jar https://github.com/open-telemetry/opentelemetry-java-instrumentation/releases/download/v${OTEL_VERSION}/opentelemetry-javaagent.jar; \
    curl -sSL -o lib/opentelemetry-api-${OTEL_VERSION}.jar https://repo1.maven.org/maven2/io/opentelemetry/opentelemetry-api/${OTEL_VERSION}/opentelemetry-api-${OTEL_VERSION}.jar; \
    curl -sSL -o lib/opentelemetry-sdk-trace-${OTEL_VERSION}.jar https://repo1.maven.org/maven2/io/opentelemetry/opentelemetry-sdk-trace/${OTEL_VERSION}/opentelemetry-sdk-trace-${OTEL_VERSION}.jar; \
    curl -sSL -o lib/opentelemetry-sdk-${OTEL_VERSION}.jar https://repo1.maven.org/maven2/io/opentelemetry/opentelemetry-sdk/${OTEL_VERSION}/opentelemetry-sdk-${OTEL_VERSION}.jar; \
    curl -sSL -o lib/opentelemetry-context-${OTEL_VERSION}.jar https://repo1.maven.org/maven2/io/opentelemetry/opentelemetry-context/${OTEL_VERSION}/opentelemetry-context-${OTEL_VERSION}.jar; \
    curl -sSL -o lib/opentelemetry-instrumentation-api-${OTEL_VERSION}.jar https://repo1.maven.org/maven2/io/opentelemetry/instrumentation/opentelemetry-instrumentation-api/${OTEL_VERSION}/opentelemetry-instrumentation-api-${OTEL_VERSION}.jar; \
    curl -sSL -o lib/opentelemetry-instrumentation-api-semconv-${OTEL_VERSION}-alpha.jar https://repo1.maven.org/maven2/io/opentelemetry/instrumentation/opentelemetry-instrumentation-api-semconv/${OTEL_VERSION}-alpha/opentelemetry-instrumentation-api-semconv-${OTEL_VERSION}-alpha.jar; \
    curl -sSL -o lib/opentelemetry-semconv-${OTEL_VERSION}-alpha.jar https://repo1.maven.org/maven2/io/opentelemetry/opentelemetry-semconv/${OTEL_VERSION}-alpha/opentelemetry-semconv-${OTEL_VERSION}-alpha.jar; \
    curl -sSL -o lib/opentelemetry-extension-trace-propagators-${OTEL_VERSION}.jar https://repo1.maven.org/maven2/io/opentelemetry/opentelemetry-extension-trace-propagators/${OTEL_VERSION}/opentelemetry-extension-trace-propagators-${OTEL_VERSION}-alpha.jar; \
    # curl -sSL -o lib/opentelemetry-opencensus-shim-${OTEL_VERSION}.jar https://repo1.maven.org/maven2/io/opentelemetry/opentelemetry-opencensus-shim/${OTEL_VERSION}-alpha/opentelemetry-opencensus-shim-${OTEL_VERSION}-alpha.jar; \
    # curl -sSL -o lib/opentelemetry-opentracing-shim-${OTEL_VERSION}.jar https://repo1.maven.org/maven2/io/opentelemetry/opentelemetry-opentracing-shim/${OTEL_VERSION}-alpha/opentelemetry-opentracing-shim-${OTEL_VERSION}-alpha.jar; 
    # curl -sSL -o lib/opencensus-impl-core-0.31.1.jar https://repo1.maven.org/maven2/io/opencensus/opencensus-impl-core/0.31.1/opencensus-impl-core-0.31.1.jar; \
    # curl -sSL -o lib/opencensus-api-0.31.1.jar https://repo1.maven.org/maven2/io/opencensus/opencensus-api/0.31.1/opencensus-api-0.31.1.jar; 
    


