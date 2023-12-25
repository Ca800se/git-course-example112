<title>Учет техники комплектующих компьютерной техники</title> <style> .title{ фон: серый; отступ: 10 пикселей; белый цвет; размер фона: обложка; ширина: 120 пикселей; граница: сплошная 4 пикселя; радиус границы: 15 пикселей; цвет границы: черный; семейство шрифтов: без засечек; размер шрифта: 20 пикселей; } .cabinet{ фон: серый; отступ: 10 пикселей; белый цвет; размер фона: обложка; ширина: 300 пикселей; граница: сплошная 4 пикселя; радиус границы: 15 пикселей; цвет границы: черный; семейство шрифтов: без засечек; размер шрифта: 20 пикселей;
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
		<tr>
		<td><?= $item[0] ?></td>
		<td><?= $item[1] ?></td>
		<td><?= $item[2] ?></td>
		<td><?= $item[3] ?></td>
		<td><?= $item[4] ?></td>
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
		<button type="submit">Добавить</button>
	</form>
</body>
