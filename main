def transcode(choice):
  result = ""
  shift = (int(input("Enter the key to shift the text back (0-26): ")) % 26)
  usertxt = input("Enter the text to transcode: ")
  for letters in usertxt:
    cnr = ord(letters.upper())
    if cnr < 65 or cnr >90:
      result += chr(cnr)
    elif cnr+(shift*choice) <= 65 or cnr+(shift*choice) >= 90:
      cnr -= (26 * choice)
      result += chr(cnr+(shift*choice))
    else:
      result += chr(cnr+(shift*choice))
  print("\nHere is your transcoded text: " + result)
  getInput()

def hello():
  print("Hello, what do you want to do?")
  print("Type 'encode' to create a secret text,\n'decode' to retrieve the original or\n'quit' or 'exit' to stop the program.")
  getInput()

def getInput():
  print("\n----------\n")
  choice = input("Tell me what to do: ")
  print("\n----------\n")

  if choice == "encode":
    transcode(1)
  elif choice == "decode":
    transcode(-1)
  elif choice == "exit" or choice == "quit":
    quit()
  else:
    getInput()

hello()
