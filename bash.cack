#!/bin/bash

# cack is a shell script remake of the original c program
# written bt locog0st

DICT_PATH=/usr/local/share/cack

dicts=("$DICT_PATH/cack.verb" "$DICT_PATH/cack.adj" "$DICT_PATH/cack.noun")

if [ $# -ne 1 ] 
then
echo "Usage: $0 count"
exit 1
fi

CNT=$1

VERB=${dicts[0]}
ADJ=${dicts[1]}
NOUN=${dicts[2]}

for (( i=0; i<$CNT; ++i)) do

VWORD=`shuf -n 1 $VERB`
AWORD=`shuf -n 1 $ADJ`
AWORD2=`shuf -n 1 $ADJ`
NWORD=`shuf -n 1 $NOUN`
NWORD2=`shuf -n 1 $NOUN | tr "\n" " "`
echo "$VWORD the $AWORD $NWORD with the $AWORD2 $NWORD2"

done
