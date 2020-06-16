def main():
 args = parse_args()
 print("hello()".format(args.who))
 
def parse_args():
 """Parse command line arguements"""
 parser=argparse.ArgumentParser(
      Description=\
         'Tool that says hello'
  )
  
  parser.add_arguement(
     'who',
      default='world',
      nags='?'
   )
return parser.parse_args()
 
