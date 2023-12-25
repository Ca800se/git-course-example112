
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<link rel="stylesheet" href="style/style.css">
	<title>Учет техники комплектующих компьютерной техники</title>
	</head>
	<style>
		.title{
			background: gray;
			padding:10px;
			color: white;
			background-size: cover;
			width: 120px;
			border: 4px solid;
			border-radius: 15px;
			border-color: black;
			font-family:sans-serif;
			font-size: 20px;
		}
		.cabinet{
			background: gray;
			padding:10px;
			color: white;
			background-size: cover;
			width: 300px;
			border: 4px solid;
			border-radius: 15px;
			border-color: black;
			font-family:sans-serif;
			font-size: 20px;

		}
		.date{
			background: gray;
			padding:10px;
			color: white;
			background-size: cover;
			width: 300px;
			border: 4px solid;
			border-radius: 15px;
			border-color: black;
			font-family:sans-serif;
			font-size: 20px;
		}
		.postavka{
			background: gray;
			padding:10px;
			color: white;
			background-size: cover;
			width: 300px;
			border: 4px solid;
			border-radius: 15px;
			border-color: black;
			font-family:sans-serif;
			font-size: 20px;

		}
		.srok{
			background: gray;
			padding:10px;
			color: white;
			background-size: cover;
			width: 300px;
			border: 4px solid;
			border-radius: 15px;
			border-color: black;
			font-family:sans-serif;
			font-size: 20px;

		}
		input, textarea, button {
  		padding: 10px;
  		display: block;
  		min-height: 30px;
  		width: 250px;
  		margin-bottom: 10px;
  		border-radius: 15px;
		}
		form{
			background-color: gray;
			padding: 20px;
			width: 400px;
			border-radius: 20px;
		}
	</style>
<body>
	<table>
		<tr>
			<th>id</th>
			<th>Техника</th>
			<th>Кабинет в котором стоит данная техника</th>
			<th>Дата когда была поставлена техника в данный кабинет</th>
			<th>Поставщик</th>
			<th>Срок доставки</th>
			<th>&#9998;</th>
			<th>&#10006;</th>
		</tr>
	
			<tr>
			<td><?= $item[0] ?></td>
			<td><?= $item[1] ?></td>
			<td><?= $item[2] ?></td>
			<td><?= $item[3] ?></td>
			<td><?= $item[4] ?></td>
			<td><?= $item[5] ?></td>
			<td><?= $item[5] ?></td>
			<td><?= $item[5] ?></td>
			<td><a href="update.php?id=<?= $item[0] ?>">Обновить</a></td>
			<td><a href="vendor/delete.php?id=<?= $item[0] ?>">Удалить</a></td>
			</tr>
		
		</table>
		<h2 class="updated">Добавить новую технику</h2>
		<form action="vendor/create.php" method="post">
			<p class="title">Название</p>
			<input type="text" name="title">
			<p class="cabinet">Кабинет в котором будет стоять техника</p>
			<input type="numeric" name="cabinet"></textarea>
			<p class="date">Дата поставки техники</p>
			<input type="date" name="date">
			<p class="postavka">Поставщик</p>
			<input type="text" name="postavka">
			<p class="srok">Срок доставки</p>
			<input type="text" name="srok">
			<button type="submit">Добавить</button>
		</form>
	</body>
</html> 
