# Introducing Python

This repository aims to outline Python programming language in QGIS and keep it short and relevant to get a solid foundation for visualizing and analyzing data.

PyQgis cookbook can be found [here](https://docs.qgis.org/testing/en/docs/pyqgis_developer_cookbook/).

It is great for users who do not have any prior programming knowledge and they want to build their knowledge gradually in QGIS. Python provides a great amount of python machine learning and analytical packages.

*Add layer.shp to QGIS.*


```python
QgsProject.instance().setCrs(QgsCoordinateReferenceSystem(26910))

layer = iface.addVectorLayer("C:\\Users\\sulova andrea\\Desktop\\Courses\\Ex_Files_QGIS_Python_AEC\Exercise Files\\1 Beginning Python\\DATA\\ROAD_CENTERLINES.shp","Roads","ogr")

layer.renderer().symbol().setColor(QColor("green"))
layer.triggerRepaint()
```
