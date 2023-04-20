# UE5-Stylized-Rendering
Some Materails for the stylized rendering in UE5
1.创建三个后处理盒子
2.BWMaterial单独放一个盒子
3.PPHatching与PPPaper放一个盒子
4.PPLineMaterial，PPLineMix与PPPaper放一个盒子
5.三个盒子尤其是PPHatching最好都不要添加体积云，会影响最终效果
6.PPHatching在编译时会报错，因为UE5不会自动添加曲线到曲线图谱中
7.将High，Mid和Low，Shadow曲线手动添加到AltasHatching图谱中
8.将曲线图谱手动添加到PPHatching材质中，并按照对应的参数名字进行添加
9.Paper123分别对应于Low，Mid，High三个曲线下的纹理
10.PPHatching盒子的exposure中的auto exposure bias（曝光补偿）应改为负值，正的曝光属性会让素描显示不出来
