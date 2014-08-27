package mahjong_solitaire.events;

import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import mahjong_solitaire.ui.MahjongSolitaireMiniGame;

/**
 *
 * @author Thomas Marion
 */
public class BackHandler implements ActionListener{
    
    private MahjongSolitaireMiniGame game;
    
    public BackHandler(MahjongSolitaireMiniGame initGame)
    {
        game = initGame;
    }
    
    @Override
    public void actionPerformed(ActionEvent ae)
    {
        game.reset();
        game.switchToSplashScreen();
    }
}
