# ExcelFromPython
Generation Of Excel Sheet From Python Using Openpyxl
from openpyxl import Workbook
import time
book = Workbook()
sheet = book.active   #worksheet. You can get sheet
sheet['A1'] = "Message Name"
sheet['B1'] = "Message ID"
sheet['C1'] = "Signal Name"
sheet['D1'] = "Length of Signal"
now = time.strftime("%x")
sheet['p1'] = now
book.save("rishavdemo1.xlsx")
