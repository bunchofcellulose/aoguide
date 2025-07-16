---
title: Significant Figures
weight: 2
---

Significant figures, are digits that carry both reliability and necessity in conveying a particular quantity.

To avoid conveying a misleading level of precision, numbers are often rounded. For instance, it would create false precision to present a measurement as 12.34525 kg when the measuring instrument only provides accuracy to the nearest gram (0.001 kg). In this case, the significant figures are the first five digits (1, 2, 3, 4, and 5) from the leftmost digit, and the number should be rounded to these significant figures, resulting in 12.345 kg as the accurate value.

## Rules to identify significant figures in a number

- Non-zero digits within the given measurement or reporting resolution are significant.
- Zeros between two significant non-zero digits are significant (significant trapped zeros).
- Zeros to the left of the first non-zero digit (leading zeros) are not significant.
- Zeros to the right of the last non-zero digit (trailing zeros) in a number with the decimal point are significant if they are within the measurement or reporting resolution.
- Trailing zeros in an integer may or may not be significant, depending on the measurement or reporting resolution.
- An exact number has an infinite number of significant figures. (If the number of apples in a bag is 4 (exact number), then this number is 4.0000... (with infinite trailing zeros to the right of the decimal point). As a result, 4 does not impact the number of significant figures or digits in the result of calculations with it.)
- A mathematical or physical constant has significant figures to its known digits.

## Rounding to significant figures

To round a number to n significant figures:

- If the n + 1 digit is greater than 5 or is 5 followed by other non-zero digits, add 1 to the n digit. For example, if we want to round 1.2459 to 3 significant figures, then this step results in 1.25.
- If the n + 1 digit is 5 not followed by other digits or followed by only zeros, then rounding requires a tie-breaking rule. For example, to round 1.25 to 2 significant figures, i. Round half away from zero rounds up to 1.3; or ii. Round half to even, which rounds to the nearest even number. With this method, 1.25 is rounded down to 1.2. If this method applies to 1.35, then it is rounded up to 1.4. This is the method preferred by many scientific disciplines, because, for example, it avoids skewing the average value of a long list of values upwards
- For an integer in rounding, replace the digits after the n digit with zeros. For example, if 1254 is rounded to 2 significant figures, then 5 and 4 are replaced to 0 so that it will be 1300. For a number with the decimal point in rounding, remove the digits after the n digit. For example, if 14.895 is rounded to 3 significant figures, then the digits after 8 are removed so that it will be 14.9.

## Significant figures in writing uncertainty

It is recommended for a measurement result to include the measurement uncertainty such as $x_\text{best} \pm \sigma_x$, where $x_\text{best}$ and $\sigma_x$ are the best estimate and uncertainty in the measurement respectively. $x_\text{best}$ can be the average of measured values and $\sigma_x$ can be the standard deviation or a multiple of the measurement deviation. The rules to write $x_\text{best} \pm \sigma_x$ are:

- $\sigma_x$ should usually be quoted to only one or two significant figures, as more precision is unlikely to be reliable or meaningful.
- The digit positions of the last significant figures in $x_\text{best}$ and $\sigma_x$ are the same, otherwise the consistency is lost. For example, "1.79 ± 0.067" is incorrect, as it does not make sense to have more accurate uncertainty than the best estimate.

## Implied uncertainty

Uncertainty may be implied by the last significant figure if it is not explicitly expressed. The implied uncertainty is $\pm$ the half of the minimum scale at the last significant figure position. For example, if the mass of an object is reported as 3.78 kg without mentioning uncertainty, then $\pm$ 0.005 kg measurement uncertainty may be implied. If the mass of an object is estimated as 3.78 ± 0.07 kg, so the actual mass is probably somewhere in the range 3.71 to 3.85 kg, and it is desired to report it with a single number, then 3.8 kg is the best number to report since its implied uncertainty ± 0.05 kg gives a mass range of 3.75 to 3.85 kg, which is close to the measurement range. If the uncertainty is a bit larger, i.e. 3.78 ± 0.09 kg, then 3.8 kg is still the best single number to quote, since if "4 kg" was reported then a lot of information would be lost.

## Arithmetic with significant figures

When performing arithmetic operations with numbers that have significant figures, the result should be rounded to the appropriate number of significant figures based on the operation performed.

- For quantities created from measured quantities via multiplication and division, the calculated result should have as many significant figures as the least number of significant figures among the measured quantities used in the calculation.
- For quantities created from measured quantities via addition and subtraction, the last significant figure position (e.g., hundreds, tens, ones, tenths, hundredths, and so forth) in the calculated result should be the same as the leftmost or largest digit position among the last significant figures of the measured quantities in the calculation.
- The base-10 logarithm of a normalized number (i.e., $a \times 10^b$ with $1 \leq a < 10$ and $b$ as an integer), is rounded such that its decimal part (called mantissa) has as many significant figures as the significant figures in the normalized number. When taking the antilogarithm of a normalized number, the result is rounded to have as many significant figures as the significant figures in the decimal part of the number to be antiloged.
