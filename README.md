# canvas_tutorial
##原生canvas相关的积累

* 常见用法或者不常见用法



>###关于什么时候用beginPath()
首先明白，canvas绘制的时机：
1.绘画的时候，如用lineTo()，arc()时，则需要执行fill()的时候进行绘制。此时记作时机a。
2.如果用fillRect()这种一次性完整成型的方式，在fillRect执行的时候，canvas便完成绘制。此时记作时机b。
时机a，时机b，绘制的时候，都需要读取canvas stage，如颜色、方法、旋转等。读取的范围就是最近的一次beginPath的时候开始。

