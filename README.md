# Introducing Python

This repository aims to outline Python programming language in QGIS and keep it short and relevant to get a solid foundation for visualizing and analyzing data.

PyQgis cookbook can be found [here](https://docs.qgis.org/testing/en/docs/pyqgis_developer_cookbook/).

It is great for users who do not have any prior programming knowledge and they want to build their knowledge gradually in QGIS. Python provides a great amount of python machine learning and analytical packages.

*Python script to open a preexisting QGIS project named as qgz or QGZ.*
```python
project.write("C:\\Users\\sulova andrea\\Desktop\\Courses\\ROAD.qgz")
QgsProject.instance().clear()

```


*Python script to open a preexisting project.*

```python
QgsProject.instance().setCrs(QgsCoordinateReferenceSystem(26910))

layer = iface.addVectorLayer("C:\\Users\\sulova andrea\\Desktop\\Courses\\ROAD.shp","Roads","ogr")

layer.renderer().symbol().setColor(QColor("green"))
layer.triggerRepaint()
```
