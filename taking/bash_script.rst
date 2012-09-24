
Read input
=====
read -t var #timeout
read -s var #hidden

If else
=====
if expression; then
    do_smt
elif
    do_smt
else
    do_smt
fi


Test expression
=====
    test expression
or
    [ expression ]

-defLrwx
-nt -ot -z -n
=
!=


Tracing
=====
set -x # enable
set +x # disable

Arithmetic
=====

$((var1 + var2))

Function
=====
function name
{
    body
}


Switch
=====
case word in
    pattern ) statements ;; # ;; mean break
    pattern ) statements ;;
    pattern ) statements
esac

Loops
=====
while expression 
do
    do_smtg
done

until expression 
do
    do_smt
done

=====
=====
=====
=====
