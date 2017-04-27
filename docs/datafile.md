# Fileformat Description that gets written as temporary file:

VERTICES:#number of vertices
x y z (of each vertex)
POLYGONS:
comma separate list of each vertid in the polygon;;materialname;;polytype (which can be FACE, SubD, or CCSS)
WEIGHT:name of weightmap
weight of vertice (in same order as VERTICES)
MORPH:name of morphmap
deltax deltay deltaz
UV:name of uvmap:number of uv coordinates
u v:polyid:pntid (for discontinuous UVs) or
u v:pntid        (for continuous UVs)

Example data format for a box:

VERTICES:8
-0.5 -0.5 -0.5
-0.5 -0.5 0.5
-0.5 0.5 0.5
-0.5 0.5 -0.5
0.5 -0.5 -0.5
0.5 -0.5 0.5
0.5 0.5 0.5
0.5 0.5 -0.5
POLYGONS:6
0,1,2,3;;Default;;FACE
0,4,5,1;;Default;;FACE
1,5,6,2;;Default;;FACE
3,2,6,7;;Default;;FACE
0,3,7,4;;Default;;FACE
4,7,6,5;;Default;;FACE
WEIGHT:simpleweights
1.0
1.0
1.0
1.0
1.0
1.0
1.0
1.0
UV:txuvmap:24
0.339743584394 0.339743584394:PLY:0:PNT:0
0.660256385803 0.339743584394:PLY:0:PNT:1
0.660256385803 0.660256385803:PLY:0:PNT:2
0.339743584394 0.660256385803:PLY:0:PNT:3
0.660256385803 0.326923072338:PLY:1:PNT:5
0.339743584394 0.326923072338:PLY:1:PNT:1
0.00641027092934 0.339743584394:PLY:3:PNT:3
0.00641027092934 0.660256385803:PLY:3:PNT:2
0.326923072338 0.660256385803:PLY:3:PNT:6
0.326923072338 0.339743584394:PLY:3:PNT:7
0.673076927662 0.00641025649384:PLY:4:PNT:0
0.993589758873 0.00641025649384:PLY:4:PNT:4
0.673076927662 0.339743584394:PLY:5:PNT:4
0.673076927662 0.660256385803:PLY:5:PNT:7
0.993589758873 0.660256385803:PLY:5:PNT:6
0.993589758873 0.339743584394:PLY:5:PNT:5
0.339743584394 0.00641025649384:PNT:0
0.660256385803 0.00641025649384:PNT:4
0.00641027092934 0.00641025649384:PNT:1
0.326923072338 0.00641025649384:PNT:5
0.326923072338 0.326923072338:PNT:6
0.00641027092934 0.326923072338:PNT:2
0.673076927662 0.326923072338:PNT:3
0.993589758873 0.326923072338:PNT:7
MORPH:simplemorph
None
None
0.0 0.290000021458 0.0
0.0 0.290000021458 0.0
None
None
0.0 0.290000021458 0.0
0.0 0.290000021458 0.0
