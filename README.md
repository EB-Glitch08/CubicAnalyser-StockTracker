# Cubic

A C# console application built for the CS0603 module at Brunel University London. It provides two core tools: a **cubic function analyser** that finds critical points (minima, maxima, and inflection points), and a **stock market data analyser** that processes historical AMD trading data from CSV.

## Features

### Cubic Function Analysis
- Input custom coefficients for any cubic function `f(x) = ax³ + bx² + cx + d`
- Evaluate the function at a given x value
- Automatically find critical points using the discriminant of the first derivative
- Classify each point as a local minimum, local maximum, or point of inflection using the second derivative test

### Stock Data Analysis
- **Yearly summary** — reads `AMD.csv` and outputs:
  - Total trading days
  - Opening and closing prices for the year
  - Price range (low–high)
  - Highest volume trading day and its closing price change
- **Monthly breakdown** — filter by January, May, or December to view:
  - Opening and closing prices for the month
  - Price range
  - Highest volume trading day

## How to Run

1. Make sure you have the [.NET SDK](https://dotnet.microsoft.com/download) installed.
2. Clone the repo:
   ```bash
   git clone https://github.com/EB-Glitch08/cubic.git
   cd cubic
   ```
3. Place your `AMD.csv` file in the project root (date format: `dd/MM/yyyy`).
4. Run the application:
   ```bash
   dotnet run
   ```

## CSV Format

The stock analyser expects a CSV with **no header row** in this format:

```
dd/MM/yyyy,Open,High,Low,Close,Volume
```

## Built With

- C# / .NET
- LINQ for data aggregation

## Author

**Emmanuel Boachie** — [EB-Glitch08](https://github.com/EB-Glitch08)
