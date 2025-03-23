class Random {// enter after the curly bracket
    static int seed;
    
    function void setSeed(int newSeed) {
        let seed = newSeed;

        return;
    }

method void drawWin() {
		if (winVariable = 0) {
			do rowWin(winRow);
		}// enter after the curly bracket
		if (winVariable = 1) {
			do colWin(winCol);
		}// enter after the curly bracket
		if (winVariable = 2) {
			do topDiagonalWin();
		}// enter after the curly bracket
		if (winVariable = 3) {
			do botDiagonalWin();
		}// enter after the curly bracket
		return;
	}

var int row, col, cell1, cell2, cell3; //bad naming variables
		let isPlayerWin = false; 
		let isDraw = false; 
		let row = 0; 
		let col = 0; 
let moves = Array.new(emptyCellsCount * 2);
		let counter = 0;// enter after ;
		while (r1 < 3) {
			let c1 = 0;
			while (c1 < 3) {
				if (boardArray[positionToIndex(r1, c1)] = 0) {
					let moves[counter] = r1;
					let moves[counter + 1] = c1;
					let counter = counter + 2;
				}
				let c1 = c1 + 1;
			}
			let r1 = r1 + 1;
		}//enter after the curly bracket
		return moves;
	}

if (gameStatus = 3) { //enter after the curly bracket
                if (currentPlayer = 0) {
                    // Won't happen with smart computer
                    // FIX: add difficulty levels
                    do Utils.showMessage("You win, enter to restart");
                } else { // enter befor else
                    do Utils.showMessage("You lost, enter to restart");
                }
                let isGameOver = true;
            }

while (i < moveCount) {
            do Game.animation();
            do board.makeMove(moveList[i + i], moveList[i + i + 1], mark);
            let nextScore = Game.getMoveScore(mark);// add enter
            if (nextScore > currentScore) {
                let currentScore = nextScore;
                let bestMove[0] = currentScore;
                let bestMove[1] = moveList[i + i];
                let bestMove[2] = moveList[i + i + 1];
            }//add enter
            do board.takeBackMove(moveList[i + i], moveList[i + i + 1]);
            let i = i + 1;
        }

if (animationIter= 600) {//what is??? backslash crush this program
        do Utils.showMessage("In progress... \");
        return;
    }
    if (animationIter= 600) {
        do Utils.showMessage("In progress... *");
        return;
    }
    if (animationIter = 500) {
        let animationIter = 0;
    }
    return;
    }

    function int getMoveScore(Mark mark) {
        var Array otherMove;
        var int otherScore;

        do board.evaluateWin();

        if (board.isDraw()) {
            return 0;
        }

        if (board.isWin()) {
            return 1;
        }

        let otherMove = Game.getBestMove(Game.getOtherMark(mark));
        let otherScore = otherMove[0];
        do otherMove.dispose();
        return -otherScore;
    }

    // Быстро получаем случайный первый ход компьютера
    function Array getRandomMove() {
        var int randomInput;
        var Array possibleMove;

        while (true) {
            let randomInput = Random.randRange(8) + 1;
            let possibleMove = Game.inputToMove(randomInput);
            if (board.isFree(possibleMove[0], possibleMove[1])) {
                return possibleMove;
            }
        }

        return possibleMove;
    }

    function void getGameSeed() {
        var int count;
        var boolean isEnterPressed;

        let isEnterPressed = false;
        let count = 1;

        while (~isEnterPressed) {
            if (Keyboard.keyPressed() = 128) {
                let isEnterPressed = true;
            }

            let count = count + 1;

            if (count > 20251) {
                let count = 1;
            }
        }

        do Random.setSeed(count);
        return;
    }
}

1) код стайл я бы подправил, перенес бы елсы и после слово class жмакал ентер и со следующей строки 
строки начиналась бы скобочка
2) в файле геймтаск неправильно слеш поставлен из-за этого все съехало
а так код нормальный





