# CSS-Utilities

Testing area for various CSS utility and component classes. I am just now getting familiar with the CUBE methodology (Andy Bell) and need a repo to save and test reusable CSS

## gamut - a generic color setter

A color utility that explicity defines a primary and secondary hue. The utility auto-generates the complement (cm) and two triadic shades (t1, t2) as well as a light and dark variant of each. Choose these colors by setting the CSS custom properties --primary and --secondary at the :root level to a specific hue in degrees. e.g. --primary: 120;

The defaults can be modified in the html if desired using a style on the html or body tag: body style="--primary: 120; --secondary: 70;"

In addition to primary and secondary, standard hues are also provided for info, success, warning and danger for use in buttons and messages.

Then use the following classes:

- background/text - to target the current background or text color (don't use both on same element).
- primary/secondary/info/success/warning/danger - to select a hue (again, dont use more than one on same element).
- cm/t1/t2 - to select the complement, triadic-1 or triadic-2 variant color (default is actual color).
- light/shade/normal/dark - to select shade (defaults to normal)

## full-bleed - escape current wrapper constraints

Class is used to temporarily escape display boundary, especially to
modify a background. May be necessary to re-wrap any contained elements
if their width is to be constrained.

## stripe - make a slanted background

Make background from background hue as a horizontal stripe angled at 2 degrees. e.g. class="stripe background primary light"
