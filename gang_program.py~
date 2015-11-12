#!/usr/bin/python

import sys, getopt

def main(argv):
   confFilePath = ''
   hexFilePath = ''
   avrDudePath=''
   try:
      opts, args = getopt.getopt(argv,"ha:c:x:")
   except getopt.GetoptError:
      print 'test.py -x <hexfile> -c <conffile> -a <avrdude path>'
      sys.exit(2)
   for opt, arg in opts:
      if opt == '-h':
         print 'test.py -x <hexfile> -c <conffile> -a <avrdude path>'
     	 sys.exit()
      elif opt in ("-x"):
         hexFilePath = arg
      elif opt in ("-c"):
         confFilePath = arg
      elif opt in ("-a"):
         avrDudePath = arg

   print 'HEX file is "', hexFilePath
   print 'CONF file is "', confFilePath
   print 'AVRdude file is "', avrDudePath
	

if __name__ == "__main__":
   main(sys.argv[1:])
