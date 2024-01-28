// Java-labs-basics-
import java.util.Scanner;

public class DistanceCalculator {
    public static void main(String[] args) {
        // اطلب إدخال إحداثيات النقطة الأولى
        Scanner scanner = new Scanner(System.in);
        System.out.println("إدخل إحداثيات النقطة الأولى:");
        System.out.print("x1: ");
        double x1 = scanner.nextDouble();
        System.out.print("y1: ");
        double y1 = scanner.nextDouble();
        System.out.print("z1: ");
        double z1 = scanner.nextDouble();

        // اطلب إدخال إحداثيات النقطة الثانية
        System.out.println("إدخل إحداثيات النقطة الثانية:");
        System.out.print("x2: ");
        double x2 = scanner.nextDouble();
        System.out.print("y2: ");
        double y2 = scanner.nextDouble();
        System.out.print("z2: ");
        double z2 = scanner.nextDouble();

        // حساب المسافة بين النقطتين
        double distance = calculateDistance(x1, y1, z1, x2, y2, z2);

        // طباعة النتيجة
        System.out.println("المسافة بين النقطتين: " + distance);

        // أغلق الماسح الضوئي
        scanner.close();
    }

    // دالة لحساب المسافة بين نقطتين
    public static double calculateDistance(double x1, double y1, double z1, double x2, double y2, double z2) {
        return Math.sqrt(Math.pow(x2 - x1, 2) + Math.pow(y2 - y1, 2) + Math.pow(z2 - z1, 2));
    }
}
