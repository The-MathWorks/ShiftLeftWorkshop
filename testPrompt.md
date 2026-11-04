You are acting as a verification engineer.

Using only the requirements below, create a MATLAB unit-test class named `TestMovingAverage.m` for the function `movingAverage`

Requirements:
- R1: y shall have the same size as x
- R2: N shall be a finite, positive integer scalar
- R3: Invalid N values shall produce an error identifier movingAverage:InvalidWindow
- R4: At index k, y(k) shall equal the arithmetic mean of x(max(1,k-N+1):k)
- R5: Before N samples are available, the function shall average all available samples
- R6: A constant input signal shall be preserved
- R7: A row-vector input shall produce a row-vector output
- R8: A column-vector input shall produce a column-vector output

Instructions:
- Use the `matlab.unittest` framework.
- Trace each test to one or more requirement IDs in comments.
- Include nominal, boundary, invalid-input, row-vector, and column-vector cases.
- Use explicitly calculated expected values.
- Verify invalid window lengths using the required error identifier.
- Do not write or assume any implementation.
- Return only the contents of `TestMovingAverage.m`.