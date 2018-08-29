/*
  Shield_Wrapper.cpp - Library for PHPoC Shield for Arduino.
  Created by Hyungjun Kim(hjkim@eztcp.com), August 24, 2018.
  Released into the public domain.
*/

#include <SPI.h>
#include <Phpoc.h>
#include "Shield_Wrapper.h"

PhpocClient __client;

Shield_Wrapper::Shield_Wrapper(){
	_status = 0;
}

void Shield_Wrapper::begin()
{
	Serial.println(F("Begin PHPoC Shield for Arduino!\n"));
	Phpoc.begin(PF_LOG_SPI | PF_LOG_NET);
}

void Shield_Wrapper::disconnect()
{
}

void Shield_Wrapper::print(){
	Serial.print(F("IP: "));Serial.println(Phpoc.localIP());
}

Client* Shield_Wrapper::getClient(){
	return (Client*)&__client;
}



