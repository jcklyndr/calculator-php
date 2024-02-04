<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	 <link rel="preconnect" href="https://fonts.googleapis.com">
	 <link rel="stylesheet" type="text/css" href="calcustyle.css">
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
	<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;500;700&display=swap" rel="stylesheet">
	<link rel="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.2.1/css/fontawesome.min.css">
	<link rel="stylesheet" type="text/css" href="calcustyle.css">
	<title>Simple Calculator</title>
</head>
<body>
<?php
$buttons = [1,2,3,'+',4,5,6,'-',7,8,9,'*','=',0,'.','/'];
$pressed = '';
if (isset($_POST['pressed'])) {
    if ($_POST['pressed'] == 'Remove') {
        $pressed = 'R';
    } elseif ($_POST['pressed'] == 'Clear') {
        $pressed = 'Clear';
    } elseif (in_array($_POST['pressed'], $buttons)) {
        $pressed = $_POST['pressed'];
    }
}
$display = '';
if (isset($_POST['display']) && preg_match('~^(?:[\\d.]+[*/+-]?)+$~', $_POST['display'], $out)) {
    $display = $out[0];
}
if ($pressed == 'Clear') {
    $display = '';
} elseif ($pressed == 'R') {
    $display = substr($display, 0, -1);
} elseif ($pressed == '=' && preg_match('~^\\d*\\.?\\d+(?:[*/+-]\\d*\\.?\\d+)*$~', $display)) {
    ob_start();
    eval("echo $display;");
    $result = ob_get_clean();
    if ($result === FALSE) {
        $display = 'Error';
    } else {
        $display = $result;
    }
} else {
    $display .= $pressed;
}
?>
<div class="container">
	<h1>SIMPLE CALCULATOR</h1>
	<div class="calculator">
<form action="" method="POST">
        <table>
        	<input type="text" name="display" value="<?php echo htmlspecialchars($display);?>" placeholder="calculate" readonly/>
            <?php foreach (array_chunk($buttons, 4) as $chunk): ?>
                <tr>
                    <?php foreach ($chunk as $button): ?>
                        <td class="button-row"<?php echo (count($chunk) != 4 ? " colspan=\"4\"" : ""); ?>><button name="pressed" value="<?php echo $button; ?>" class="btnval"><?php echo $button; ?></button></td>
                    <?php endforeach; ?>
                </tr>
            <?php endforeach; ?>
        </table><br>
        <div class="button-roww">
                    <button type="submit" name="pressed" id="btn"value="Remove" >Remove</button>
                    <button type="submit" name="pressed"  id="btn"value="Clear" >Clear</button>
                </div>
        <input type="hidden" name="stored" value="<?php echo $display; ?>">
    </form><br>
</div><br>
</div>
</body>
</html>
