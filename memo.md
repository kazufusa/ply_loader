# PLY format

[PLY format](https://jp.mathworks.com/help/vision/ug/the-ply-format.html)

[TextureDouble.ply](https://github.com/cnr-isti-vclab/meshlabjs/blob/master/mesh/textured/TextureDouble.ply)

```
ply
format ascii 1.0
comment VCGLIB generated
comment TextureFile <this>_A.png # texture file path 0
comment TextureFile <this>_B.png # texture file path 1
element vertex 8
property float x
property float y
property float z
element face 4
property list uchar int vertex_indices  # meshtype(3:triangle, 4:rectangle, ...), vertex No1, vertex No2,...
property list uchar float texcoord      # num, (x, y), (x, y), ... for texture path coordinates
property int texnumber                  # texture file path indices (0 or 1 in this case)
end_header
0 0 0  # 点0
1 0 0  # 点1
1 1 0  # 点2
0 1 0  # 点3
2 0 0  # 点4
3 0 0  # 点5
3 1 0  # 点6
2 1 0  # 点7
3 0 1 2 6 0 0 1 0 1 1 0 # 3なので三角形メッシュ1, vertex_index*3, 6, texture(x,y)*3, texture file index
3 0 2 3 6 0 0 1 1 0 1 0 # 3なので三角形メッシュ2
3 4 5 6 6 0 0 1 0 1 1 1 # 3なので三角形メッシュ3
3 4 6 7 6 0 0 1 1 0 1 1 # 3なので三角形メッシュ4
```



# ref

[PCX](https://github.com/keijiro/Pcx)
