# AircraftHud


changes in FlyingPawn

FlyingBP/Blueprints/FlyingPawn
	FlyingPawn/Default/SpringArmLength:	0
	FlyingPawn/Default/SpringArmOffset:	-20; 0; 60
	Add Component under Mesh: BP_HudWidgetComponent
	PlaneMesh/BP_HudWidgetComponent/Transform: X,Z as required, Rota-Z_ 180, Scale All 0,1
	PlaneMesh/BP_HudWidgetComponent/Materials: MI_HudWidget3dOpaque
	PlaneMesh/BP_HudWidgetComponent/UserInterface/DrawSize:	1920 x 1080
	Add Event-Caller for Pitch/Roll/Yaw-Change in Graph



