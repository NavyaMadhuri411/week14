# Experiment 14: ReAct Agent Using LangGraph and Gemini

## Aim
To build a simple LLM agent using LangGraph's `create_react_agent`, with tools for live weather retrieval and mathematical calculations.

## Problem Statement
Create an agent that retrieves the current temperature in London, converts Celsius to Fahrenheit, calculates 15% of 320, and adds the calculation result to the Fahrenheit temperature.

## Tools and Technologies
- Python
- Google Gemini API
- LangGraph
- LangChain
- Open-Meteo weather API
- Google Colab

## Algorithm
1. Install the required Python packages.
2. Configure the Gemini API key.
3. Define a safe calculator tool.
4. Define a weather tool that returns the current temperature in Celsius.
5. Initialize the Gemini language model with temperature 0.
6. Create a ReAct agent using `create_react_agent`.
7. Invoke the agent with the hardcoded query.
8. Display tool calls, observations, and the final answer.
9. Save the execution trace in `output.txt`.

## Test Query
What is the current temperature in London in Fahrenheit? Also calculate 15% of 320 and add it to the temperature.

## Expected Calculations
- Celsius to Fahrenheit: `C × 9 / 5 + 32`
- Percentage: `320 × 15 / 100 = 48`
- Combined total: Fahrenheit temperature + 48

The actual total depends on the temperature returned by the weather service.

## Conclusion
This experiment demonstrates a ReAct agent that combines live information retrieval and arithmetic tools to complete a multi-step task. The agent uses tool outputs to construct its final answer.
