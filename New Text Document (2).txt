package com.itt.manifesto;

import java.io.IOException;
import java.net.ServerSocket;
import java.net.Socket;

public class Tester {
	public static void main(String[] args) throws IOException {
		
		int portNO = Integer.parseInt(args[0]);

		ServerSocket socket = new ServerSocket(portNO);
		System.out.println("ServerSocket =" + socket);
		Socket s = socket.accept();
		System.out.println("Socket =" + s);
		socket.close();
		
	}
}
