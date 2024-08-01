using Photon.Pun;
using UnityEngine;

public class PlayfabReload : MonoBehaviour
{
    public bool Reload;
    public Playfablogin playfablogin;

    private void Update()
    {
        if (Reload)
        {
            playfablogin.Login();
            Reload = false;
            Debug.Log("Logged in");
        }
    }
}
