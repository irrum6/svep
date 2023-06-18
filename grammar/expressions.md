--TAble Variables
x = operation

examples:

names = @shop $ name$ ;

or

names = $ name$ @shop ;

-- Variables

x = value;

examples:

x = 5;

this x  then can be resolved by ? operator

@shop::objects::paint $ color $ [quantity > ?x];

-- Aliases
x = @identity;

examples:

paint = @shop::objects::paint;

aliases are accessed @? operator (combinatioan of identity and variable resolver operators)

@?paint $ color $ [quantity > ?x];

