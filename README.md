# Financial-Concepts-in-Python
---
## Description

  * In this jupyter notebook, I have explained the basic principles of Finance. 
  * How these basic principles are essential for making important financial decisions.
---
## Python Libraries used
 
  * Numpy
  * Numpy Financial
---
## Contents

 1. **PART-1** : Fundamental financial concepts like the time value of money, growth and rate of return, compound interest, discount factors, depreciation, and inflation.
 
    - **Growth and Rate of Return**
    - **Compound Interest** : Both time and the rate of return are very important variables when forecasting the future value of an investment. Another important variable is the number of compounding periods, which can greatly affect compounded returns over time.
    - **Discount Factors and Depreciation** : Growth rates are often unpredictable in finance rather than constant, and can even be negative, leading to depreciation, which simply means a declining value over time. Unfortunately, not everything grows in value over time. In fact, many assets depreciate, or lose value over time. To simulate this, we can simply assume a negative expected rate of return.
      - **What is Discount Factor ?** : If we know the depreciated value of an investment and the depreciation rate, but we want to calculate the initial value of the investment? Using simple algebra, we can build a formula to derive the discount factor (df), which is the number that when multiplied by the future value, equals the initial value of the investment.
    - **Present value and Future Value**
      - **Numpy financial package**
      - There is a module called numpy-financial which contains 10 functions which will make our life much easier when working with financial values.
      - Installing package - `pip install numpy-financial`
      - **Present Value** : The `.pv(rate, nper, pmt, fv)` function, for example, allows to calculate the present value of an investment as before with a few simple parameters:    
        ```
        rate: The rate of return of the investment
        nper: The lifespan of the investment
        pmt: The (fixed) payment at the beginning or end of each period (which is 0 in our example)
        fv: The future value of the investment
        ```
      - **Future Value** : The numpy-financial module also contains a similar function, `.fv(rate, nper, pmt, pv)`, which allows to calculate the future value of an investment as before with a few simple parameters:
        ```
        rate: The rate of return of the investment
        nper: The lifespan of the investment
        pmt: The (fixed) payment at the beginning or end of each period (which is 0 in our example)
        pv: The present value of the investment
        ```
      - **Inflation Rate** : Adjusting future values for inflation

        First, forecast the future value of an investment given a rate of return.

        Second, discount the future value of the investment by a projected inflation rate.
        
    - **Net Present Value and Cash Flows**
      - **Cash Flows** : Cash Flows are a series of gains or losses from an investment over time.
      - **Discounting Cash flows**
      - **Diminishing Cash flows**
      
 2. **PART-2** : Project Proposals and Cash flow projections
    - **Internal Rate of Return**
    - **Debt and Equity financing**
    - **WACC - Weighted Average Cost of Capital**
    - **Comparing project NPV with IRR**
    - **Two projects with different lifespans**
    - **Equivalent Annual Annuity (EAA) Approach** : The equivalent annual annuity (EAA) approach allows us to compare two projects by essentially assuming that each project is an investment generating a flat interest rate each year (an annuity), and calculating the annual payment we would receive from each project, discounted to present value.
    
