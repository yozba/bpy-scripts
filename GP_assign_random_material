import bpy
import numpy as np

for a in bpy.context.selected_objects:
	bpy.context.view_layer.objects.active = a
	activeObjData = bpy.context.active_object.data

	stroke_num = len(activeObjData.layers[0].frames[0].strokes)
	material_num = len(activeObjData.materials)

	for i in range(stroke_num):
		matIndex = np.random.randint(0, material_num - 1)
		activeObjData.layers[0].frames[0].strokes[i].material_index = matIndex
