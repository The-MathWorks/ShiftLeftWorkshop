You are acting as an implementation engineer.

Implement the MATLAB function `movingAverage.m` from the following requirements:

- R1: y shall have the same size as x
- R2: N shall be a finite, positive integer scalar
- R3: Invalid N values shall produce an error identifier movingAverage:InvalidWindow
- R4: At index k, y(k) shall equal the arithmetic mean of x(max(1,k-N+1):k)
- R5: Before N samples are available, the function shall average all available samples
- R6: A constant input signal shall be preserved
- R7: A row-vector input shall produce a row-vector output
- R8: A column-vector input shall produce a column-vector output

The existing verification tests are fixed and must not be modified. The unit test suite is in Test/TestMovingAverage.m

Instructions:
- Create `movingAverage.m` and avoid using any built-in functions.
- Exception due to invalid `N` is specified in the description of R3.
- Satisfy every stated requirement.
- Use clear, deterministic MATLAB code.
- Preserve the size and orientation of the input vector.
- Use the required error identifier for invalid N values.
- Do not modify, weaken, or bypass any test.
- Return only the contents of `movingAverage.m`.