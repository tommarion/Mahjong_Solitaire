package mahjong_solitaire.events;

import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import mahjong_solitaire.MahjongSolitaire.MahjongSolitairePropertyType;
import mahjong_solitaire.data.MahjongSolitaireDataModel;
import mahjong_solitaire.ui.MahjongSolitaireMiniGame;

/**
 * This event handler responds to when the user requests to
 * undo a mover in-game. 
 * 
 * @author Thomas Marion
 */
public class UndoHandler implements ActionListener
{
 // HERE'S THE GAME WE'LL UPDATE
    private MahjongSolitaireMiniGame game;
    private MahjongSolitaireDataModel data;
    
    /**
     * This constructor just stores the game for later.
     * 
     * @param initGame the game to update
     */
    public UndoHandler(MahjongSolitaireMiniGame initGame)
    {
        game = initGame;
    }
    
    /**
     * Here is the event response. This code is executed when
     * the user clicks on the button for undo move. Note that the game 
     * data is already locked for this thread before it is called, 
     * and that it will be unlocked after it returns.
     * 
     * @param ae the event object for the button press
     */
    @Override
    public void actionPerformed(ActionEvent ae)
    {
        data = (MahjongSolitaireDataModel)game.getDataModel();
        data.undoLastMove();
    }
}
