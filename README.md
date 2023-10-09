# repo excel_tips

Just a placeholder for tips in data assuance and quality testing done in Excel

# split name into separate cells

FIRST NAME: 
  =LEFT(A2, FIND(" ",A2)-1)
  =LEFT(A2, SEARCH(" ",A2)-1)

LAST NAME
  =RIGHT(A2, LEN(A2)-FIND(" ",A2))
  =RIGHT(A2, LEN(A2)-SEARCH(" ",AZ))


## extract n characters after certain character

  =MID(A2,4,3)


## Find Something in Square Brackets

  =MID(C2,FIND("[",C2)+1, SUM(FIND({"[","]"},C2)*{-1,1})-1)

 
## Find in Parenthesis

  =MID(C2,FIND("(",E1)+1, SUM(FIND({"(",")"},C2)*{-1,1})-1)


## String to the right of a hyphen

=MID(A1,SEARCH("-",A1,SEARCH("-",A1)+1)+1,256)


## A has a short search string, B col has long text to return if match occurs

<TODO> Finish bringing over all tips </TODO>

