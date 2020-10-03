---
layout: post
title:  "Random chess game"
description: "Random chess game"
excerpt: "Random chess game"
permalink: /random-chess-game/
date:   2020-10-02
published: true
tags: chess
tags_visible: true
show_in_blog: false
comments: true
---

# Chess!

<div id="myBoard" style="width: 300px"></div>
<button onclick="doChessMoves(board, game, ['e4', 'e5', 'Nf3', 'f5'], 1000)">Moves 1</button>
<button onclick="doChessMoves(board, game, ['d4', 'fxe4', 'Nxe5', 'Nf6'], 1000)">Moves 2</button>
<button onclick="showRandomGame(board, game)">Random</button>

<script type="text/javascript">
	game = new Chess();
	board = Chessboard('myBoard', 'start');
</script>