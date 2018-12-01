import flash.events.MouseEvent;
import flash.display.Stage;
import flash.utils.Timer;
import flash.sensors.Accelerometer;
import adobe.utils.XMLUI;
import flash.ui.Multitouch;
import flash.ui.MultitouchInputMode;
import flash.ui.Multitouch
import flash.events.GestureEvent
import flash.events.TransformGestureEvent
import flash.events.PressAndTapGestureEvent

Multitouch.inputMode = MultitouchInputMode.TOUCH_POINT;
Multitouch.inputMode = MultitouchInputMode.GESTURE;
var indexArrow: Arrow = new Arrow();


var grabArrowFlag = false;

var tenThousands: int = 0;
var numOfficers: int = 101;
var avgSalary: int = 51000;
var change: int = 0;
var newNumOfficers: int = 0;
var percentage: int = 0;
var total:int;

var numOfficersTF: TextField = new TextField();
var avgSalaryTF: TextField = new TextField();
var changeTF: TextField = new TextField();
var newNumOfficersTF: TextField = new TextField();
var percentageTF: TextField = new TextField();


var tenThousandsSTF: TextField = new TextField();
var numOfficersSTF: TextField = new TextField();
var avgSalarySTF: TextField = new TextField();
var changeSTF: TextField = new TextField();
var newNumOfficersSTF: TextField = new TextField();
var percentageSTF: TextField = new TextField();


var numOfficersTFF: TextFormat = new TextFormat();
var avgSalaryTFF: TextFormat = new TextFormat();
var changeTFF: TextFormat = new TextFormat();
var newNumOfficersTFF: TextFormat = new TextFormat();
var percentageTFF: TextFormat = new TextFormat();

var tenThousandsSTFF: TextFormat = new TextFormat();
var numOfficersSTFF: TextFormat = new TextFormat();
var avgSalarySTFF: TextFormat = new TextFormat();
var changeSTFF: TextFormat = new TextFormat();
var newNumOfficersSTFF: TextFormat = new TextFormat();
var percentageSTFF: TextFormat = new TextFormat();


numOfficersTF.name = "numOfficersTF";
avgSalaryTF.name = "avgSalaryTF";
changeTF.name = "changeTF";
newNumOfficersTF.name = "newNumOfficersTF";
percentageTF.name = "percentageTF";
tenThousandsSTF.name = "tenThousandsSTF";
numOfficersSTF.name = "numOfficersSTF";
avgSalarySTF.name = "avgSalarySTF";
changeSTF.name = "changeSTF";
newNumOfficersSTF.name = "newNumOfficersSTF";
percentageSTF.name = "percentageSTF";




initialize();

function initialize(): void {
	stage.addEventListener(Event.ENTER_FRAME, arrowMovement); // constantly running
	indexArrow.x = 362;
	indexArrow.y = 132;
	addChild(indexArrow);
	indexArrow.addEventListener(MouseEvent.CLICK, arrowClicked);
	indexArrow.addEventListener(PressAndTapGestureEvent.GESTURE_PRESS_AND_TAP, touchTapped);
	
}

function arrowMovement(event: Event): void {
	if (grabArrowFlag == true) {
		indexArrow.y = (stage.mouseY);
		//trace(stage.mouseY);
		checkPosition();
		upDateNumbers();
		upDateText();
		if(indexArrow.y <= 130){indexArrow.y = 130;}
		if(indexArrow.y >= 498){indexArrow.y = 498;}
		addChild(indexArrow);
	}
}

function arrowClicked(event: MouseEvent): void {
	stage.addEventListener(MouseEvent.MOUSE_UP, mouseButtonReleased);
	indexArrow.removeEventListener(MouseEvent.CLICK, arrowClicked);
	indexArrow.removeEventListener(PressAndTapGestureEvent.GESTURE_PRESS_AND_TAP, touchTapped);
	grabArrowFlag = true;

}

function touchTapped(event: TouchEvent): void {
	indexArrow.addEventListener(PressAndTapGestureEvent.GESTURE_PRESS_AND_TAP, released);
	indexArrow.removeEventListener(MouseEvent.CLICK, arrowClicked);
	indexArrow.removeEventListener(PressAndTapGestureEvent.GESTURE_PRESS_AND_TAP, touchTapped);
	grabArrowFlag = true;

}

function mouseButtonReleased(event: MouseEvent): void {
	grabArrowFlag = false;
	stage.removeEventListener(MouseEvent.MOUSE_UP, mouseButtonReleased);
	indexArrow.addEventListener(MouseEvent.CLICK, arrowClicked);
}

function released(event: TouchEvent): void {
	grabArrowFlag = false;
	stage.removeEventListener(MouseEvent.MOUSE_UP, mouseButtonReleased);
	indexArrow.removeEventListener(PressAndTapGestureEvent.GESTURE_PRESS_AND_TAP, touchTapped);
	
}

function checkPosition(): void {
	if (indexArrow.y <= 1601) {
		tenThousands = 00000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 161 && indexArrow.y <= 180) {
		tenThousands = 10000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 181 && indexArrow.y <= 200) {
		tenThousands = 20000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 201 && indexArrow.y <= 220) {
		tenThousands = 30000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 221 && indexArrow.y <= 240) {
		tenThousands = 40000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 241 && indexArrow.y <= 260) {
		tenThousands = 50000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 261 && indexArrow.y <= 280) {
		tenThousands = 60000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 281 && indexArrow.y <= 300) {
		tenThousands = 70000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 301 && indexArrow.y <= 320) {
		tenThousands = 80000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 321 && indexArrow.y <= 340) {
		tenThousands = 90000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 341 && indexArrow.y <= 360) {
		tenThousands = 100000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 361 && indexArrow.y <= 380) {
		tenThousands = 110000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 381 && indexArrow.y <= 400) {
		tenThousands = 120000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 401 && indexArrow.y <= 420) {
		tenThousands = 130000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 421 && indexArrow.y <= 440) {
		tenThousands = 140000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 441 && indexArrow.y <= 460) {
		tenThousands = 150000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 461 && indexArrow.y <= 480) {
		tenThousands = 160000;
		upDateNumbers();
		upDateText();
	}
	if (indexArrow.y >= 481) {
		tenThousands = 170000;
		upDateNumbers();
		upDateText();
	}
	

}

function upDateNumbers(): void {

}

function upDateText(): void {

	removeOldText();



	numOfficersTFF.font = "Arial";
	numOfficersTFF.size = 84;
	numOfficersTFF.color = 0x00FF00;
	numOfficersTFF.rightMargin = 10;
	numOfficersTF.border = false;
	numOfficersTF.x = 587;
	numOfficersTF.y = 130;
	numOfficersTF.autoSize = TextFieldAutoSize.RIGHT;
	numOfficersTF.text = numOfficers.toString();
	numOfficersTF.setTextFormat(numOfficersTFF);
	addChild(numOfficersTF);
	// he following is no longer average salary but total officers
	avgSalaryTFF.font = "Arial";
	avgSalaryTFF.size = 84;
	avgSalaryTFF.color = 0x00FF00;
	avgSalaryTFF.rightMargin = 10;
	avgSalaryTF.border = false;
	avgSalaryTF.x = 587;
	avgSalaryTF.y = 348;
	avgSalaryTF.autoSize = TextFieldAutoSize.RIGHT;
	total = newNumOfficers + numOfficers; 
	avgSalaryTF.text = total.toString();
	avgSalaryTF.setTextFormat(avgSalaryTFF);
	addChild(avgSalaryTF);
	changeTFF.font = "Arial";
	changeTFF.size = 84;
	changeTFF.color = 0x00FF00;
	changeTFF.rightMargin = 10;
	changeTF.border = false;
	changeTF.x = 587;
	changeTF.y = 230;
	changeTF.autoSize = TextFieldAutoSize.RIGHT;
	//changeTF.text = change.toString();
	changeTF.setTextFormat(changeTFF);
	addChild(changeTF);
	newNumOfficersTFF.font = "Arial";
	newNumOfficersTFF.size = 84;
	newNumOfficersTFF.color = 0x00FF00;
	newNumOfficersTFF.rightMargin = 10;
	newNumOfficersTF.border = false;
	newNumOfficersTF.x = 681;
	newNumOfficersTF.y = 235;
	newNumOfficersTF.autoSize = TextFieldAutoSize.RIGHT;
	newNumOfficersTF.text = newNumOfficers.toString();
	newNumOfficersTF.setTextFormat(newNumOfficersTFF);
	addChild(newNumOfficersTF);
	percentageTFF.font = "Arial";
	percentageTFF.size = 84;
	percentageTFF.color = 0x00FF00;
	percentageTFF.rightMargin = 10;
	percentageTF.border = false;
	percentageTF.x = 587;
	percentageTF.y = 455;
	percentageTF.autoSize = TextFieldAutoSize.RIGHT;
	percentage = (((newNumOfficers * numOfficers) / 100) + 100);
	percentageTF.text = percentage.toString();
	percentageTF.setTextFormat(percentageTFF);
	addChild(percentageTF);
	tenThousandsSTFF.font = "Arial";
	tenThousandsSTFF.size = 23;
	tenThousandsSTFF.color = 0x00FF00;
	tenThousandsSTFF.rightMargin = 10;
	tenThousandsSTF.border = false;
	tenThousandsSTF.x = 278;
	tenThousandsSTF.y = 73;
	tenThousandsSTF.autoSize = TextFieldAutoSize.RIGHT;
	tenThousandsSTF.text = tenThousands.toString();
	tenThousandsSTF.setTextFormat(tenThousandsSTFF);
	addChild(tenThousandsSTF);
	numOfficersSTFF.font = "Arial";
	numOfficersSTFF.size = 23;
	numOfficersSTFF.color = 0x00FF00;
	numOfficersSTFF.rightMargin = 10;
	numOfficersSTF.border = false;
	numOfficersSTF.x = 395;
	numOfficersSTF.y = 73;
	numOfficersSTF.autoSize = TextFieldAutoSize.RIGHT;
	numOfficersSTF.text = numOfficers.toString();
	numOfficersSTF.setTextFormat(numOfficersSTFF);
	addChild(numOfficersSTF);
	avgSalarySTFF.font = "Arial";
	avgSalarySTFF.size = 23;
	avgSalarySTFF.color = 0x00FF00;
	avgSalarySTFF.rightMargin = 5;
	avgSalarySTF.border = false;
	avgSalarySTF.x = 611;
	avgSalarySTF.y = 73;
	avgSalarySTF.autoSize = TextFieldAutoSize.RIGHT;
	avgSalarySTF.text = avgSalary.toString();
	avgSalarySTF.setTextFormat(avgSalarySTFF);
	addChild(avgSalarySTF);
	changeSTFF.font = "Arial";
	changeSTFF.size = 23;
	changeSTFF.color = 0x00FF00;
	changeSTFF.rightMargin = 0;
	changeSTF.border = false;
	changeSTF.x = 469;
	changeSTF.y = 73;
	change = tenThousands * numOfficers;
	avgSalarySTF.autoSize = TextFieldAutoSize.LEFT;
	changeSTF.text = change.toString();
	if(change >= 9970000 && change <= 11100000){changeSTF.text = "10.1 Mil";}
	if(change >= 10240000 && change <= 12100000){changeSTF.text = "11.1 Mil";}
	if(change >= 11210000 && change <= 13170000){changeSTF.text = "12.1 Mil";}
	if(change >= 12280000 && change <= 14100000){changeSTF.text = "13.1 Mil";}
	if(change >= 13250000 && change <= 15100000){changeSTF.text = "14.1 Mil";}
	if(change >= 14220000 && change <= 16100000){changeSTF.text = "15.1 Mil";}
	if(change >= 15490000 && change <= 17100000){changeSTF.text = "16.1 Mil";}
	if(change >= 16490000){changeSTF.text = "17.1 Mil";}
	changeSTF.setTextFormat(changeSTFF);
	addChild(changeSTF);
	newNumOfficersSTFF.font = "Arial";
	newNumOfficersSTFF.size = 23;
	newNumOfficersSTFF.color = 0x00FF00;
	newNumOfficersSTFF.rightMargin = 10;
	newNumOfficersSTF.border = false;
	newNumOfficersSTF.x = 712;
	newNumOfficersSTF.y = 73;
	newNumOfficersSTF.autoSize = TextFieldAutoSize.RIGHT;
	newNumOfficers = change / avgSalary;
	newNumOfficersSTF.text = newNumOfficers.toString();;
	newNumOfficersSTF.setTextFormat(newNumOfficersSTFF);
	addChild(newNumOfficersSTF);
}

function removeOldText():void{
if(contains(numOfficersTF)){numOfficersTF.parent.removeChild(numOfficersTF);}
if(contains(avgSalaryTF)){avgSalaryTF.parent.removeChild(avgSalaryTF);}
if(contains(changeTF)){changeTF.parent.removeChild(changeTF);}
if(contains(newNumOfficersTF)){newNumOfficersTF.parent.removeChild(newNumOfficersTF);}
if(contains(percentageTF)){percentageTF.parent.removeChild(percentageTF);}
if(contains(tenThousandsSTF)){tenThousandsSTF.parent.removeChild(tenThousandsSTF);}
if(contains(numOfficersSTF)){numOfficersSTF.parent.removeChild(numOfficersSTF);}
if(contains(avgSalarySTF)){avgSalarySTF.parent.removeChild(avgSalarySTF);}
if(contains(changeSTF)){changeSTF.parent.removeChild(changeSTF);}
if(contains(newNumOfficersSTF)){newNumOfficersSTF.parent.removeChild(newNumOfficersSTF);}
if(contains(percentageSTF)){percentageSTF.parent.removeChild(percentageSTF);}
}
