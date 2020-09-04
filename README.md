# CSS-Utilities

Testing area for various CSS utility and component classes. I am just now getting familiar with the CUBE methodology (Andy Bell) and need a repo to save and test reusable CSS

## gamut - a generic color setter

A color utility that explicity defines a primary and secondary hue. The utility auto-generates the complement (cm) and two triadic shades (t1, t2) as well as a light and dark variant of each. Choose these colors by setting the CSS custom properties --primary and --secondary at the :root level to a specific hue. e.g. --primary: 120deg;

In addition to primary and secondary, standard hues are also provided for info, success, warning and danger for use in buttons and messages.

Then use the following classes:
- background/text - to target the current background or text color (don't use both on same element).
- primary/secondary/info/success/warning/danger - to select a hue (again, dont use more than one on same element).
- cm/t1/t2 - to select the complement, triadic-1 or triadic-2 variant color (default is actual color).
- light/shade/normal/dark - to select shade (defaults to normal)

