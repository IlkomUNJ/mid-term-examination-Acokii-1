window size is depending on the line width, if the width is 4 so the ideal window size to recognize is 12x12 matrix. in my code i set the line width to 1 so the matrix goes from 12x12 to 3x3.

or we can use a 3x3 matrix which have 4x4 matrix inside. for each 4x4 matrix with full true condition is recognize as a pixel with non-white. then to detect the segment we check around it. but it's different for each line created. if the line is straight horizontal or vertical the pattern is either horizontal true matrix value or vertical true matrix value. The diagonal line will produce left side identity matrix or right side identity matrix.

horizontal	vertical	diagonal
0 0 0		0 1 0		1 0 0		0 0 1
1 1 1		0 1 0		0 1 0	or	0 1 0
0 0 0		0 1 0		0 0 1		1 0 0
