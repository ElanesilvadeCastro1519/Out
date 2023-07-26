# Out
import RPi.GPIO as GPIO import time  # Configuração dos pinos GPIO.setmode(GPIO.BCM) GPIO.setup(18, GPIO.OUT)  # Função para ligar a bomba de água def ligar_bomba(tempo):     GPIO.output(18, GPIO.HIGH)     time.sleep(tempo)     GPIO.output(18, GPIO.LOW)
