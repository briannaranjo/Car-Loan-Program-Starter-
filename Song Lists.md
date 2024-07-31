import java.util.Arrays;
import java.util.ArrayList;

class Playlist {
  public static void main(String[] args){
    String[] favoriteSongs = {"Song 1", "Song 2","Song 3","Song 4","Song 5","Song 6","Song 7","Song 8","Song 9","Song 10"};
    System.out.println(favoriteSongs[0]);
    System.out.println(favoriteSongs[1]);
    System.out.println(favoriteSongs[2]);

    ArrayList<String> desertIslandPlaylist = new ArrayList<>();
    desertIslandPlaylist.add("Song 1.1");
    desertIslandPlaylist.add("Song 2.1");
    desertIslandPlaylist.add("Song 3.1");
    desertIslandPlaylist.add("Song 4.1");
    desertIslandPlaylist.add("Song 5.1");

    System.out.println(desertIslandPlaylist);

    desertIslandPlaylist.addAll(Arrays.asList(favoriteSongs));

    System.out.println(desertIslandPlaylist.size());

    desertIslandPlaylist.remove("Song 1");
    desertIslandPlaylist.remove("Song 2");
    desertIslandPlaylist.remove("Song 3");
    desertIslandPlaylist.remove("Song 4");
    desertIslandPlaylist.remove("Song 5");
    desertIslandPlaylist.remove("Song 6");
    desertIslandPlaylist.remove("Song 7");
    desertIslandPlaylist.remove("Song 8");
    desertIslandPlaylist.remove("Song 9");
    desertIslandPlaylist.remove("Song 10");

    System.out.println(desertIslandPlaylist);

    System.out.println(desertIslandPlaylist.indexOf("Song 2.1"));
    System.out.println(desertIslandPlaylist.indexOf("Song 5.1"));

    int SongA = desertIslandPlaylist.indexOf("Song 2.1");
    int SongB = desertIslandPlaylist.indexOf("Song 5.1");

    String tempA = "Song A";

    desertIslandPlaylist.set(SongA, "Song 5.1");

    System.out.println(desertIslandPlaylist);

    desertIslandPlaylist.set(SongB, "Song A");

    System.out.println(desertIslandPlaylist);
    
  }
}
