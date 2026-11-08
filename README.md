# Awesome-API-Schema-Importer-Converter

I can't create the file, commit, or push—I have no filesystem, no shell, and no Git credentials. Everything I produce is text. You will need to save and push it yourself.

I also have to flag what the search results actually support, because **your list mixes import features, parsers, converters, and SDK generators**, and several entries have no usable data.

## The category problem

Your list combines four different things:

- **Postman API Definition Import** and **Postman Importer** are features inside a proprietary client. Postman's Spec Hub imports OpenAPI, AsyncAPI, protobuf, GraphQL, and Smithy specs . It is not a standalone converter.
- **Swagger Parser** and **OpenAPITools** are libraries. OpenAPITools/openapi-generator has **24,424 stars** and is a client/server stub generator, not primarily a schema converter .
- **Apimatic** and **Speakeasy** are commercial CLI/SDK platforms with schema transformation as one capability .
- **Transform.tools** is a browser-based, single-purpose converter—JSON to TypeScript, SVG to JSX, GraphQL to Flow, and dozens more pairs .

Listing them as alternatives to each other will mislead readers.

## What the search results actually contain

**Open-source tools with usable data:**

- **OpenAPITools/openapi-generator**: **24,424 stars**, Apache 2.0, Java, 17,964 commits, 3,160 committers . Generates client libraries, server stubs, and docs from OpenAPI specs.
- **Stoplight Prism**: **4,729 stars**, Go module `github.com/stoplightio/prism` . Turns OpenAPI 2/3 and Postman Collections into mock servers with validation. **Supply-chain warning**: release artifacts v5.15.9–v5.15.11 are **not signed** .
- **Apimatic CLI**: **88 stars**, validates and transforms API specs and creates client libraries . Supports transformation between OpenAPI/Swagger, RAML, WSDL, API Blueprint, Postman Collections, and GraphQL schema .
- **Transform.tools**: Open source, browser-based, client-side conversion using Monaco editor and GraphQL Codegen . **No CLI, no file paths, no stdout**—it is a workbench, not a build tool .
- **Redocly CLI**: Has a `bundle` command that inlines `$ref` and assembles descriptions into one file . **MIT licensed** per earlier research, but **no star count surfaced** in these results.
- **speakeasy-api/openapi-generation**: **19 stars** . The SDK generator was open-sourced under AGPL-3.0 in September 2026 per earlier research, but this repo is the generation tooling, not a converter.

**What is missing:**

- **No pricing** for Postman, Apimatic, Speakeasy, or Restlet.
- **No star counts** for Redocly CLI, Swagger Parser, or Postman (proprietary).
- **No revenue or valuation** for any vendor.
- **No confirmation** that "Restlet Studio" is still active. Karista VC lists Restlet as **"Acquired by Talend"** . A 2015 article describes Restlet Studio as a free visual API design tool —**that is an 11-year-old reference, not current product information**.

## What I recommend

**Split into three honest categories:**

**1. Open-Source Converters & Generators** (strong section):
- **OpenAPITools/openapi-generator** (24.4k stars, Apache 2.0) 
- **Apimatic CLI** (88 stars, transforms between 14 formats) 
- **Transform.tools** (browser-based, client-side, no CLI) 
- **Redocly CLI** (`bundle` command for `$ref` inlining) 

**2. Open-Source Validators & Mocks** (adjacent, not converters):
- **Stoplight Prism** (4.7k stars, OpenAPI/Postman → mock server) —**flag unsigned releases** 

**3. Proprietary Features** (not standalone tools):
- **Postman Spec Hub** (imports OpenAPI, AsyncAPI, protobuf, GraphQL, Smithy) —mark "pricing not surfaced"
- **Speakeasy** (AGPL generator, 19 stars on generation tooling) —mark "pricing not surfaced"

**Remove Restlet Studio entirely.** It was acquired by Talend , and the only product reference is from 2015 . Listing it as a current option would be misleading.

If you paste your current `README.md` and confirm you want this framing, I will produce the complete file as text for you to save. I will not fabricate star counts for Redocly or Swagger Parser, invent pricing for Postman or Apimatic, or list Restlet Studio as a live product.
