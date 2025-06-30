# 🚗 Vehicle Price Consultation – FIPE API Integration
A Java project developed with Spring Framework to simulate and enhance the experience of consulting average vehicle prices based on the Brazilian FIPE table.

This challenge project mirrors the official FIPE website flow while adding useful improvements like full-year evaluations and terminal-based interaction.

🎯 Project Overview
The goal of this project is to build a command-line application that:

Requests the user to select the type of vehicle: car, motorcycle, or truck.

Lists all brands available for the selected category and allows the user to choose one by its code.

Displays all vehicle models for that brand.

Prompts the user to enter a partial model name (e.g., "PALIO").

Filters and displays only the models that match the input.

Once a specific model is selected, it retrieves all available years and shows a price evaluation for each year — unlike the official FIPE website, which only displays one at a time.

🚀 Technologies & Tools
Java 17

Spring Framework (CLI-based)

Jackson for JSON deserialization

HTTP API consumption with native Java tools

Collections, Streams, and Loops for data processing

Scanner for interactive command-line input

🌐 API Integration
The project interacts with the FIPE Public API to fetch real-time data:

Vehicle types:

https://parallelum.com.br/fipe/api/v1/carros/marcas

https://parallelum.com.br/fipe/api/v1/motos/marcas

https://parallelum.com.br/fipe/api/v1/caminhoes/marcas

Models by brand:

https://parallelum.com.br/fipe/api/v1/[tipo]/marcas/{brandCode}/modelos

Available years by model:

https://parallelum.com.br/fipe/api/v1/[tipo]/marcas/{brandCode}/modelos/{modelCode}/anos

Price evaluation by year:

https://parallelum.com.br/fipe/api/v1/[tipo]/marcas/{brandCode}/modelos/{modelCode}/anos/{yearCode}

📌 Key Features
✅ Full API-driven workflow for cars, motorcycles, and trucks

✅ Dynamic filtering of models by partial name input

✅ Lists price evaluations for all years at once — improving user experience

✅ Structured and clean code using object-oriented principles

✅ JSON parsing and data modeling using Jackson and Java record classes

✅ Focused on code readability, testability, and real-world API consumption

💡 What This Project Demonstrates
Ability to consume and process complex external APIs

Efficient use of Java’s functional features (Streams, Lambdas, etc.)

Clean modeling of domain entities (brands, models, vehicles)

Hands-on understanding of data flow and API chaining

Terminal-based UX with a logical and user-friendly step-by-step flow

Building maintainable and extensible backend applications

✅ Example Use Case
The user selects cars, filters models with the keyword PALIO, selects a model, and instantly views price evaluations from every available year — a much richer experience than the original FIPE website.

This challenge not only showcases technical mastery over Java and Spring but also reflects problem-solving ability, API design understanding, and a focus on real user needs — all key skills for backend development roles.
