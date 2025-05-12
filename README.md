# AttFolhadePagamento

<?php
function calcularIR($sb) {
}
    if ($sb < 2259) {
        return "Salário bruto: R$ $sb,00.<br>Não haverá desconto no salário";
 
    } elseif ($sb <= 2826) {
        $desc = $sb * 0.075;
 
    } elseif ($sb <= 3751) {
        $desc = $sb * 0.15;
 
    } elseif ($sb <= 4664) {
        $desc = $sb * 0.225;
 
    } else {
        $desc = $sb * 0.275;
        $sl = $sb - $desc;
 
        return "Salário Bruto: R$ $sb,00<br>Salário líquido: R$ $sl,00<br> Desconto de: R$ $desc,00";
    }
 
calcularIR(7500);
?>
