# Version 1.0

SKETCH={{ cookiecutter.project_name }}.ino
COMPLEMENTS=
FQBN=Maixduino:k210:mduino
PORT=/dev/ttyUSB0
BAUDRATE=115200

# https://arduino.github.io/arduino-cli/0.35/getting-started/

build: $(SKETCH) $(COMPLEMENTS)
	arduino-cli compile --fqbn $(FQBN) --build-path build 

compile: $(SKETCH) $(COMPLEMENTS)
	arduino-cli compile --fqbn $(FQBN) 

run:
	kflash -p $(PORT) build/$(SKETCH).bin

monitor:
	arduino-cli monitor -p $(PORT) -c baudrate=$(BAUDRATE)

clear:
	rm -r build

all: compile run monitor
