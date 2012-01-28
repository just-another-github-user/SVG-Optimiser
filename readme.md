Python program to clean up SVG files, particularly those created by Inkscape or Illustrator

# Decimal places
    Rewrite attributes to a given number of decimal places.
    Strips out unnecessary trailing zeros.
    
    - Attributes
    	x, y, x1, y2, x2, y2
    	cx, cy
    	r, rx, ry
    	width, height

# Transformations
	Applies transformations to elements so the attribute can be removed.

    - Translation
        - In the form
            comma: (12,34)
            space(s): (12 34) or (12     34)
            comma and space(s): (12, 34), (12 ,34), (12 , 34) or (12  ,   34)
            decimal: (1.2, 3.4)
            negative: (-1.2, -3.4)
            
        - Shapes
            rect
            circle
            line
            
# Remove attributes
	Remove attributes with a given name, e.g. remove id attributes, which often aren't used.
    
--- To do ---

# Decimal places    
    - Attributes
    	<polyline> points
    	<path> d

# Transformations

    - Translation
        - In the form
            single: (12)
    
        - Shapes
            path
            polygon
            g
            text
            tspan
            
    - Rotation
        - Shapes
            path
            polyline
            line
            circle
            rect -> polygon?
            
    - Scale
        - Shapes
            path
            polyline
            line
            rect
            circle -> ellipse?
            
# CSS stlying
    Convert individual element styles to CSS styling where appropriate.
    Ideally find most efficient way to class elements for styling